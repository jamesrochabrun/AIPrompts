# AI Prompts Documentation

Comprehensive documentation of system prompts, tools, and workflows for major AI coding assistants.

## Overview

This repository contains detailed documentation extracted from the system prompts and API payloads of leading AI coding tools. Each directory provides both human-readable documentation and raw API structures for reference and implementation.

## Projects Documented

### 1. Codex (OpenAI)
Open-source agentic coding interface - terminal-based coding assistant

**Location**: `Codex/`

**Files**: 6 files + README
- 1 main instruction file (23KB)
- 5 tool definitions (shell, apply_patch, update_plan, code_review, view_image)

**Characteristics**:
- Concise, direct, friendly personality
- Focus on preamble messages (8-12 words)
- Plan-based task management
- Patch-based code modifications
- Approval workflow support

**Key Tools**:
- Terminal command execution
- Unified diff patching
- Plan creation and tracking
- Code review and analysis
- Image viewing

---

### 2. ClaudeCode (Anthropic)
Anthropic's official CLI for Claude - comprehensive coding assistant

**Location**: `ClaudeCode/`

**Structure**: Two complementary folders

#### ClaudeCode/BreakDown/ (37 files)
Human-readable documentation organized by category:
- **system_instructions/** (6 files) - Core behavioral guidelines
- **system_reminders/** (4 files) - Contextual hints
- **tool_usage_policies/** (4 files) - Tool usage guidelines
- **tools/** (17 files) - Individual tool documentation
- **git_workflows/** (3 files) - Git operation workflows
- **environment/** (3 files) - Environment information

#### ClaudeCode/Data/ (22 files)
Raw JSON API structures:
- System prompts (exact API payload format)
- System reminders (raw reminder text)
- Tool definitions (complete JSON schemas for 17 tools)

**Characteristics**:
- Professional objectivity focus
- TodoWrite for task management
- Specialized vs general tool preference
- Explore agent for codebase navigation
- Plan mode for review before execution

**Key Tools**:
- Task/Agent delegation (6 agent types)
- File operations (Read, Edit, Write, Glob, Grep)
- Web tools (WebFetch, WebSearch)
- Interactive questioning (AskUserQuestion)
- Background process management
- Jupyter notebook editing

---

## File Statistics

### Total Files: 71
- Codex: 6 tool/instruction files + 1 README
- ClaudeCode BreakDown: 37 documentation files + 1 README
- ClaudeCode Data: 22 raw JSON files + 1 README
- Project READMEs: 3

### Total Documentation Size
- Codex: ~33KB of prompt/tool definitions
- ClaudeCode: ~5,000+ lines of documentation

## Comparison: Codex vs ClaudeCode

### Similarities
- Both use tool-based architectures
- Both support terminal/bash operations
- Both emphasize clear communication
- Both have planning capabilities
- Both prioritize safety and user approval

### Key Differences

| Aspect | Codex | ClaudeCode |
|--------|-------|------------|
| **Tools** | 5 tools | 17 tools |
| **Code Edits** | Unified diff patches | Direct string replacement |
| **Planning** | update_plan tool | TodoWrite tool |
| **Personality** | Concise, light, curious | Professional, objective |
| **Communication** | Preambles (8-12 words) | Varied, context-dependent |
| **Agent System** | No sub-agents | 6 specialized agents |
| **Web Access** | No | Yes (fetch + search) |
| **Interactive UI** | No | Yes (AskUserQuestion) |

### Codex Strengths
- Simpler tool set (easier to understand)
- Patch-based editing (preserves context)
- Lightweight, focused approach
- Clear preamble guidelines

### ClaudeCode Strengths
- More comprehensive tool set
- Agent delegation for complex tasks
- Web access for current information
- Better file operation tools (Glob, Grep)
- Interactive question UI
- Plan mode for review
- Background process management

## Use Cases

### For Learning
- Study how major AI coding assistants work
- Understand system prompt engineering
- Compare different approaches to tool design
- See real-world examples of agent architectures

### For Implementation
- Reference for building custom AI assistants
- Tool API design patterns
- System prompt structures
- Safety and approval mechanisms

### For Integration
- Understand capabilities and constraints
- Plan integrations with existing tools
- Compare feature sets
- Evaluate which system fits your needs

## File Formats

### Codex
- Plain text files with tool definitions
- JSON schemas embedded in text
- Markdown-formatted instructions

### ClaudeCode
- **BreakDown**: Human-readable .txt documentation
- **Data**: Raw JSON structures from API payloads
- Parallel structure for learning + implementation

## Documentation Approach

Both projects follow similar organizational principles:
1. **Standalone files** - Each concept in its own file
2. **Clear descriptions** - Every file has overview and purpose
3. **Examples** - Practical usage examples included
4. **Cross-references** - Related files linked together
5. **Plain text** - Easy to read, search, and version control

## Repository Structure

```
AIPrompts/
├── README.txt                    (This file)
│
├── Codex/                        (OpenAI's Codex CLI)
│   ├── README.txt
│   ├── instructions.txt          (Main system prompt)
│   ├── shell.txt                 (Terminal commands)
│   ├── apply_patch.txt           (Code modifications)
│   ├── update_plan.txt           (Planning tool)
│   ├── code_review.txt           (Code analysis)
│   └── view_image.txt            (Image viewing)
│
└── ClaudeCode/                   (Anthropic's Claude Code)
    ├── README.txt
    │
    ├── BreakDown/                (Human-readable docs)
    │   ├── system_instructions/
    │   ├── system_reminders/
    │   ├── tool_usage_policies/
    │   ├── tools/
    │   ├── git_workflows/
    │   └── environment/
    │
    └── Data/                     (Raw JSON structures)
        ├── README.txt
        ├── System prompts
        ├── System reminders
        └── Tool definitions
```

## Contributing

This repository documents existing systems. To add new AI coding assistant documentation:

1. Create a new directory for the assistant
2. Include raw prompts/API structures
3. Optionally add organized/annotated versions
4. Follow the existing file naming patterns (.txt)
5. Include a README explaining the structure

## Sources

- **Codex**: OpenAI's open-source Codex CLI project
- **ClaudeCode**: Anthropic's Claude Code API payloads and system prompts

## License

This repository contains documentation of existing AI systems. The original prompts and tools are property of their respective creators (OpenAI, Anthropic). This documentation is provided for educational and reference purposes.

## Maintenance

Last updated: October 2025

These documents represent snapshots of the systems at the time of extraction. AI coding assistants are rapidly evolving, so check official documentation for the latest capabilities.

## Related Resources

- [OpenAI Codex CLI](https://github.com/openai/codex-cli) - Official repository
- [Claude Code Documentation](https://docs.claude.com/en/docs/claude-code) - Official docs
- [Anthropic API](https://docs.anthropic.com/) - Claude API documentation
