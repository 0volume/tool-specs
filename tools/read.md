## read
**Purpose:** Read file contents from the workspace filesystem

**When to use:**
- Viewing any file in the workspace
- Reading source code, configs, or documentation
- Getting context before making changes

**Inputs:**
- `file_path` (string, required): Path to file relative or absolute
- `limit` (number, optional): Max lines to read
- `offset` (number, optional): Line number to start from (1-indexed)

**Outputs:**
- File contents as text (truncated to 2000 lines or 50KB)

**Examples:**
```
read file_path: "TOOLS.md"
read file_path: "memory/2026-02-17.md", limit: 50
```

**Pitfalls:**
- Large files are truncated - use offset/limit for large files
- Binary files may show as garbled text
- Path must be accurate - no glob expansion

**Related tools:**
- write (for creating/updating files)
- edit (for making precise changes)
