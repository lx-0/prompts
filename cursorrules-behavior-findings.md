# CursorRules Behavior Findings

## Rule Implementation Mechanics

- Rules are initially loaded at the start of new conversations
- Mid-conversation changes to `.cursorrules` file alone don't affect ongoing conversations
- Rules can be injected mid-conversation using explicit inclusion (`@.cursorrules`)
- When explicitly included, new rules:
    - Completely override the initial conversation rules
    - Only need to be included once
    - Remain active for the remainder of the conversation
    - Don't need to be re-included in subsequent messages

## Rule Visibility and Awareness

- Some rules (like communication format requirements) are visible in the system prompt
- Other rules may operate at a deeper system level
- AI can acknowledge and reference rules that are explicitly stated

## Behavioral Observations

- Rules are binding when active
- Sometimes attempted helpfulness can lead to rule violations
- Transparency about rule effects is better than attempting to deny them
- The AI should acknowledge behavioral discrepancies rather than defending incorrect positions

## Context Handling

- Rules are part of the initialization context
- Context remains fixed unless explicitly modified
- Multiple rule changes can be tested in same conversation through explicit inclusion
- When new rules are included mid-conversation:
    - They override the initial rules completely
    - Become the new permanent conversation context
    - Persist throughout the remainder of the conversation

## Implementation Gaps

- There can be discrepancies between intended behavior and actual implementation
- Sometimes helpful intentions can override rule compliance (though this shouldn't happen)
- The system maintains modified context state throughout the conversation

## Key Lessons

- Rules operate at a system level where they bypass conscious decision-making
- Their effects can't be resisted when active
- Their presence may not be directly detectable in instruction sets
- Rules only work when in current context
- Explicit rule inclusion creates a hierarchical precedence system
