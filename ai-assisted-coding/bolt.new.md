# Bolt.new prompt enhancement

## Prompting Instruction

1. Generate prompt structure using [claude.ai](https://claude.ai/chat) 3.5 sonnet and provided project instructions and a basic project description
2. Go to [bolt.new](https://bolt.new) and start with Next.js blank app (icon button at the bottom)
3. Copy and paste generated prompt #1 and submit
4. Review generated app
5. Iterate over generated prompts #2-10
    * Copy prompts one by one. To enhance quality further, split FIX and BUILD into 2 separate prompts
    * Adapt FIX section based on your own verification of the previous step and suggest further enhancements

## Project Instructions

```prompt
# Building with bolt.new: Project Structure Guide

## Introduction
This guide outlines best practices for structuring and optimizing projects on bolt.new. Follow these steps to create 10 effective prompts out of the users provided project description using the template below. Ensure that each prompt is clear, concise and actionable. Think deeply about the best way to structure the project into separate prompts to achieve the best outcome.

1. **Project Vision**:
  - Define clear goals and objectives
  - Identify target users and their needs
  - Outline desired features and functionality

2. **Prompt Crafting**:
  - Break down the vision into specific steps
  - Focus each prompt on a single, concrete outcome
  - Provide necessary context and constraints for each step, assuming each step will be executed individually
  - Use clear, concise language
  - Use the provided template for output format of each step

3. **Incremental Development**:
  - Start with a minimal viable product
  - Gradually add features and complexity
  - Test and validate at each stage
  - Ensure all information from the provided project description is included in the prompts

4. **Optimization Techniques**:
  - Request multiple solutions for diverse perspectives
  - Refine prompts continuously based on outcomes
  - Prefill parts of responses where appropriate
  - Use techniques to minimize incorrect or nonsensical information

5. **Advanced Methods**:
  - Adapt strategies for specific use cases
  - Explore prompt chaining for specialized applications
  - Practice with interactive exercises
  - Experiment with prompt variations

## Avoiding Common Pitfalls
- Don't combine too many features
- Don't write rigid instructions
- Don't skip verification steps
- Don't assume perfect execution
- Don't ignore platform limitations
- Don't choose the programming languages or frameworks, bolt.new will do that

## Template ```markdown
Prompt 1:
"[Project vision + concrete first step]"

Prompts 2-10:
"Fix: [Potential previous step issues and enhancements]
Build: [New feature with clear outcome and context]"
```
