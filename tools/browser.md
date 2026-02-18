## browser
**Purpose:** Control web browser for automation and scraping

**When to use:**
- JavaScript-rendered pages
- Interactive web apps
- Complex navigation

**Inputs:**
- `action` (string, required): status/start/stop/snapshot/navigate/act
- `profile` (string, optional): chrome/openclaw
- `targetUrl` (string, optional): URL to navigate
- `request` (object, optional): Actions like click, type

**Outputs:**
- Page snapshot or action result

**Examples:**
```
browser action: "snapshot"
browser action: "navigate", targetUrl: "https://example.com"
browser action: "act", request: {"kind": "click", "ref": "button1"}
```

**Pitfalls:**
- Slower than web_fetch
- Can be blocked by anti-bot
- Complex to get right selectors

**Best Practices:**
- Use web_fetch first for simple pages
- Use snapshot to find elements
- Be careful with timing

**Related tools:**
- web_fetch (for simple pages)
- web_search (to find URLs)
