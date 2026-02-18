## edit
**Purpose:** Make precise, surgical edits to existing files by replacing exact text

**When to use:**
- Modifying specific parts of a file
- Safe alternative to write (preserves rest of file)
- When you know the exact text to replace

**Inputs:**
- `file_path` (string, required): File to edit
- `oldText` (string, required): Exact text to find and replace
- `newText` (string, required): Text to replace with

**Outputs:**
- Confirmation of edit

**Examples:**
```
edit file_path: "TOOLS.md", oldText: "## Current", newText: "## Updated"
```

**Pitfalls:**
- **EXACT MATCH REQUIRED**: Whitespace, newlines must match exactly
- If oldText not found, edit fails
- No undo - changes are immediate
- Can break files if replacement is malformed

**Related tools:**
- write (for full file replacement)
- read (to verify content before editing)
