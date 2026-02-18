## write
**Purpose:** Create new files or overwrite existing files completely

**When to use:**
- Creating new files from scratch
- Completely replacing a file's content
- Creating directories (automatically creates parent dirs)

**Inputs:**
- `content` (string, required): Content to write
- `file_path` (string, required): Path to write to

**Outputs:**
- Confirmation of bytes written

**Examples:**
```
write file_path: "test.md", content: "# Hello"
```

**Pitfalls:**
- **DESTRUCTIVE**: Overwrites entire file - use edit for modifications
- No confirmation before overwrite
- Doesn't merge with existing content

**Related tools:**
- read (for viewing before writing)
- edit (for safe modifications)
