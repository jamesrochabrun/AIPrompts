# ClaudeCode Prompts Documentation

Organized documentation of Claude Code's system instructions, reminders, tools, and workflows.

## Directory Structure

```
ClaudeCode/
├── system_instructions/     (6 files)
│   ├── tone_and_style.txt
│   ├── professional_objectivity.txt
│   ├── task_management.txt
│   ├── code_references.txt
│   ├── security_policy.txt
│   └── file_creation_policy.txt
│
├── system_reminders/        (4 files)
│   ├── todo_list_empty.txt
│   ├── claude_md_context.txt
│   ├── plan_mode_active.txt
│   └── system_reminder_header.txt
│
├── tool_usage_policies/     (4 files)
│   ├── tool_usage_general.txt
│   ├── parallel_tool_execution.txt
│   ├── specialized_tools_preference.txt
│   └── explore_agent_usage.txt
│
├── tools/                   (17 files)
│   ├── task.txt
│   ├── bash.txt
│   ├── glob.txt
│   ├── grep.txt
│   ├── read.txt
│   ├── edit.txt
│   ├── write.txt
│   ├── notebook_edit.txt
│   ├── web_fetch.txt
│   ├── web_search.txt
│   ├── todo_write.txt
│   ├── ask_user_question.txt
│   ├── exit_plan_mode.txt
│   ├── bash_output.txt
│   ├── kill_shell.txt
│   ├── skill.txt
│   └── slash_command.txt
│
├── git_workflows/           (3 files)
│   ├── git_commit.txt
│   ├── git_pr.txt
│   └── git_safety.txt
│
└── environment/             (3 files)
    ├── environment_info.txt
    ├── model_info.txt
    └── git_status.txt
```

## Total Files: 37

## Categories

### System Instructions (6 files)
Core behavioral guidelines for Claude Code:
- Communication style and tone
- Professional objectivity principles
- Task management with TodoWrite
- Code reference formatting
- Security constraints
- File creation policies

### System Reminders (4 files)
Contextual hints that appear during operation:
- Empty todo list reminders
- User global instructions from ~/.claude/CLAUDE.md
- Plan mode constraints
- General system reminder format

### Tool Usage Policies (4 files)
Guidelines for effective tool usage:
- General tool usage principles
- Parallel vs sequential execution
- Preference for specialized tools over bash
- When to use Explore agent

### Tools (17 files)
Individual documentation for each tool:
- Task - Launch specialized agents
- Bash - Execute shell commands
- Glob - Find files by pattern
- Grep - Search code contents
- Read - Read files
- Edit - Edit existing files
- Write - Create new files
- NotebookEdit - Edit Jupyter notebooks
- WebFetch - Fetch and analyze web content
- WebSearch - Search the web
- TodoWrite - Manage todo lists
- AskUserQuestion - Interactive questioning
- ExitPlanMode - Exit plan mode
- BashOutput - Read background shell output
- KillShell - Terminate background shells
- Skill - Execute skills
- SlashCommand - Execute slash commands

### Git Workflows (3 files)
Specialized workflows for git operations:
- Creating commits
- Creating pull requests
- Git safety protocols

### Environment (3 files)
Environment and context information:
- Working directory, platform, date
- Model identification and knowledge cutoff
- Git repository status

## File Format
All files are plain text (.txt) for easy reading and reference.

## Usage
Each file is standalone and contains:
- Clear description of the instruction/reminder/tool
- Usage guidelines and examples
- Edge cases and constraints
- Related file references

## Purpose
This structure makes it easy to:
- Reference individual components
- Update specific policies without affecting others
- Compose custom Claude Code configurations
- Understand the full scope of capabilities
- Study how Claude Code works internally

## Related
Based on the same approach as the Codex project for consistency and organization.
