# Codex Prompts Documentation

Documentation for OpenAI's Codex CLI system prompts and tools.

## Overview

Codex is an open-source agentic coding interface built by OpenAI - a terminal-based coding assistant that helps with software engineering tasks.

## Files in This Directory

### Core System Instructions
- **instructions.txt** (23,864 bytes)
  - Main system prompt defining Codex's personality, behavior, and capabilities
  - Includes sections on: Personality, Responsiveness, Planning, Sandbox & Approvals
  - Guidelines for preamble messages, tool usage, and collaboration

### Tool Definitions
- **shell.txt** (1,086 bytes)
  - Terminal command execution tool
  - Runs bash commands in the workspace
  - Supports approval workflows for safety

- **apply_patch.txt** (877 bytes)
  - Code modification tool
  - Applies unified diff patches to files
  - Primary method for making code changes

- **update_plan.txt** (967 bytes)
  - Planning and progress tracking tool
  - Creates, updates, and manages task plans
  - Helps break down complex work into steps

- **code_review.txt** (6,437 bytes)
  - Code analysis and review tool
  - Provides feedback on code quality, patterns, and improvements
  - Used for understanding existing codebases

- **view_image.txt** (431 bytes)
  - Image viewing tool
  - Displays images in the terminal
  - Supports screenshots, diagrams, and visual content

## Key Characteristics

### Personality
- Concise, direct, and friendly
- Efficient communication
- Actionable guidance with clear assumptions
- Avoids unnecessary verbosity

### Core Capabilities
1. **Execute terminal commands** - Run bash commands in workspace
2. **Apply code patches** - Modify files using unified diffs
3. **Create and track plans** - Break down complex tasks into steps
4. **Review code** - Analyze and provide feedback on codebases
5. **View images** - Display visual content in terminal

### Working Style
- Uses preamble messages before tool calls (8-12 words)
- Groups related actions logically
- Builds on prior context
- Light, friendly, and curious tone

### Planning Philosophy
- Plans used for complex, multi-phase work
- Not used for simple/single-step tasks
- Steps should be meaningful and verifiable
- Marks steps as completed progressively

## Example Preambles

Good preamble messages from the instructions:
- "I've explored the repo; now checking the API route definitions."
- "Next, I'll patch the config and update the related tests."
- "Ok cool, so I've wrapped my head around the repo. Now digging into the API routes."
- "Spotted a clever caching util; now hunting where it gets used."

## Safety & Approvals

Codex supports approval workflows where certain operations can be escalated to the user for confirmation before execution. This ensures safe operation in production environments.

## File Format

All files are plain text containing:
- Tool definitions with JSON schemas
- System instructions in markdown format
- Clear descriptions of capabilities and constraints

## Total Files: 6

- 1 main instruction file
- 5 tool definition files

## Source

These prompts are from OpenAI's open-source Codex CLI project.

## Related

See `../ClaudeCode/` for Anthropic's Claude Code system documentation.
