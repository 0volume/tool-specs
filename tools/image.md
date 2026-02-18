## image
**Purpose:** Analyze images using the configured image model

**When to use:**
- Understanding diagrams, screenshots, photos
- Visual research
- Debugging UI issues

**Inputs:**
- `image` (string, required): Image path or URL
- `prompt` (string, required): What to analyze
- `model` (string, optional): Override default model

**Outputs:**
- Text analysis of the image

**Examples:**
```
image image: "screenshot.png", prompt: "What does this UI show?"
```

**Pitfalls:**
- Requires image to be accessible
- Large images may be truncated
- Not all formats supported

**Best Practices:**
- Use clear, focused prompts
- Describe what you're looking for

**Related tools:**
- web_fetch (for getting images from URLs)
