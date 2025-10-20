# ClaudeCode Data - Raw JSON Definitions

This folder contains the exact JSON structures from Claude Code API payloads.

## Contents

### System Prompts (2 files)
- `system_prompt_1.txt` - Initial system block identifying Claude Code
- `system_prompt_2.txt` - Main system block with all instructions and guidelines

### System Reminders (3 files)
- `system_reminder_todo_empty.txt` - Empty todo list reminder
- `system_reminder_claude_md.txt` - User's global CLAUDE.md instructions
- `system_reminder_plan_mode.txt` - Plan mode constraints

### Tool Definitions (17 files)
Each file contains the exact JSON tool definition as it appears in the API:
- `task_tool.txt` - Task/Agent tool
- `bash_tool.txt` - Bash command execution
- `glob_tool.txt` - File pattern matching
- `grep_tool.txt` - Code search
- `read_tool.txt` - File reading
- `edit_tool.txt` - File editing
- `write_tool.txt` - File writing
- `notebook_edit_tool.txt` - Jupyter notebook editing
- `web_fetch_tool.txt` - Web content fetching
- `web_search_tool.txt` - Web searching
- `todo_write_tool.txt` - Todo list management
- `ask_user_question_tool.txt` - Interactive questioning
- `exit_plan_mode_tool.txt` - Plan mode exit
- `bash_output_tool.txt` - Background shell output
- `kill_shell_tool.txt` - Shell termination
- `skill_tool.txt` - Skill execution
- `slash_command_tool.txt` - Slash command execution

## Format

Each file contains the raw JSON structure exactly as it appears in the Claude Code API payload.

### Tool Files Structure
```json
{
  "name": "ToolName",
  "description": "Tool description...",
  "input_schema": {
    "type": "object",
    "properties": { ... },
    "required": [ ... ]
  }
}
```

### System Prompt Files Structure
```json
{
  "type": "text",
  "text": "...",
  "cache_control": {
    "type": "ephemeral"
  }
}
```

### System Reminder Files
```
<system-reminder>
Reminder text...
</system-reminder>
```

## Purpose

These files represent the RAW data from Claude Code API payloads, useful for:
- Understanding exact API structure
- Reference for building custom implementations
- Comparing with official API documentation
- Analyzing tool capabilities and constraints

## Related

See `../BreakDown/` for human-readable documentation and organized breakdown of these definitions.
