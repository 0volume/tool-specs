## web_search
**Purpose:** Search the web using Brave Search API

**When to use:**
- Finding information on any topic
- Researching papers, tools, concepts
- Getting current information

**Inputs:**
- `query` (string, required): Search query
- `count` (number, optional): Results to return (1-10)
- `freshness` (string, optional): pd/pw/pm/py for time filtering
- `country` (string, optional): Region-specific results

**Outputs:**
- Array of search results with title, URL, snippet

**Examples:**
```
web_search query: "agentic AI research papers", count: 5
web_search query: "MCP protocol", freshness: "pw"
```

**Pitfalls:**
- Results may not be authoritative
- snippets can be misleading - always verify
- Rate limits may apply
- Commercial results may appear

**Best Practices:**
- Verify URLs before adding to research
- Check multiple sources
- Use freshness for current topics

**Related tools:**
- web_fetch (get full page content)
