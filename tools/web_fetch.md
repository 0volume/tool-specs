## web_fetch
**Purpose:** Fetch and extract readable content from a URL (HTML to markdown/text)

**When to use:**
- Getting article content
- Extracting paper abstracts
- Reading documentation

**Inputs:**
- `url` (string, required): HTTP/HTTPS URL to fetch
- `extractMode` (string, optional): "markdown" or "text"
- `maxChars` (number, optional): Truncate at limit

**Outputs:**
- Extracted content in requested format

**Examples:**
```
web_fetch url: "https://arxiv.org/abs/2602.14922"
web_fetch url: "https://github.com/openclaw/openclaw", maxChars: 5000
```

**Pitfalls:**
- Some sites block scraping
- JavaScript-rendered content may not load
- maxChars truncates - may miss end of article
- Rate limits may apply

**Best Practices:**
- Always verify paper URLs with web_fetch before adding to archive
- Use for extracting key info, not full documents
- Check content quality after fetch

**Related tools:**
- web_search (find URLs to fetch)
