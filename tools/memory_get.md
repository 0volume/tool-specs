## memory_get
**Purpose:** Read specific snippet from memory files

**When to use:**
- After memory_search to get full context
- Reading specific memory entries
- Getting detailed context

**Inputs:**
- `path` (string, required): File path (MEMORY.md or memory/*.md)
- `from` (number, optional): Line to start
- `lines` (number, optional): Number of lines

**Outputs:**
- Requested memory snippet

**Examples:**
```
memory_get path: "MEMORY.md"
memory_get path: "memory/2026-02-17.md", from: 1, lines: 50
```

**Pitfalls:**
- Need correct path
- Line numbers must be accurate
- Can get truncated results

**Best Practices:**
- Use memory_search first to find what you need
- Be specific with from/lines

**Related tools:**
- memory_search (find what to read)
- read (for viewing full files)
