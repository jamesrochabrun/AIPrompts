# ClaudeCode Prompts Documentation

Complete documentation of Claude Code system prompts, tools, and workflows.

## Structure

```
ClaudeCode/
├── BreakDown/           Human-readable documentation
│   ├── system_instructions/    (6 files)
│   ├── system_reminders/        (4 files)
│   ├── tool_usage_policies/     (4 files)
│   ├── tools/                   (17 files)
│   ├── git_workflows/           (3 files)
│   └── environment/             (3 files)
│
└── Data/                Raw JSON definitions from API
    ├── System prompts           (2 files)
    ├── System reminders         (3 files)
    └── Tool definitions         (17 files)
```

## BreakDown Folder

Human-readable documentation organized by category:

### system_instructions/ (6 files)
Core behavioral guidelines:
- tone_and_style.txt
- professional_objectivity.txt
- task_management.txt
- code_references.txt
- security_policy.txt
- file_creation_policy.txt

### system_reminders/ (4 files)
Contextual hints during operation:
- todo_list_empty.txt
- claude_md_context.txt
- plan_mode_active.txt
- system_reminder_header.txt

### tool_usage_policies/ (4 files)
Guidelines for effective tool usage:
- tool_usage_general.txt
- parallel_tool_execution.txt
- specialized_tools_preference.txt
- explore_agent_usage.txt

### tools/ (17 files)
Individual tool documentation:
- task.txt, bash.txt, glob.txt, grep.txt
- read.txt, edit.txt, write.txt
- notebook_edit.txt, web_fetch.txt, web_search.txt
- todo_write.txt, ask_user_question.txt, exit_plan_mode.txt
- bash_output.txt, kill_shell.txt
- skill.txt, slash_command.txt

### git_workflows/ (3 files)
Specialized git workflows:
- git_commit.txt
- git_pr.txt
- git_safety.txt

### environment/ (3 files)
Environment information:
- environment_info.txt
- model_info.txt
- git_status.txt

## Data Folder

Raw JSON definitions from Claude Code API payloads:

### System Prompts (2 files)
- system_prompt_1.txt - "You are Claude Code..."
- system_prompt_2.txt - Main instructions

### System Reminders (3 files)
- system_reminder_todo_empty.txt
- system_reminder_claude_md.txt
- system_reminder_plan_mode.txt

### Tool Definitions (17 files)
Exact JSON tool definitions:
- task_tool.txt through slash_command_tool.txt

## Usage

### For Learning
- Read BreakDown files for understanding concepts
- See organized, human-readable explanations

### For Implementation
- Use Data files for exact API structures
- Reference for building custom implementations

### For Reference
- Compare BreakDown and Data to understand both the "what" and "how"
- Cross-reference between human docs and raw JSON

## Total Files

- BreakDown: 37 files
- Data: 22 files
- Total: 59 files + 3 READMEs

## Based On

This structure follows the same approach as the Codex project for consistency.
