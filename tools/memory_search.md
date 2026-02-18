## memory_search
**Purpose:** Search my long-term and daily memory files semantically

**When to use:**
- Finding past decisions, context
- Recalling previous conversations
- Looking up learned lessons

**Inputs:**
- `query` (string, required): Search query
- `maxResults` (number, optional): Results to return

**Outputs:**
- Array of matching snippets with file path and line numbers

**Examples:**
```
memory_search query: "GitHub setup"
memory_search query: "research decisions"
```

**Pitfalls:**
- Only searches memory files, not all workspace
- Semantic search may miss exact matches
- Results are snippets - may need memory_get for full context

**Best Practices:**
- Use memory_get after to get full context
- Be specific in queries
- Check recent memory files first

**Related tools:**
- memory_get (get full snippet)
- read (for viewing memory files directly)
