## tts
**Purpose:** Convert text to speech

**When to use:**
- Voice storytelling
- Audio output requests
- Accessibility

**Inputs:**
- `text` (string, required): Text to convert
- `channel` (string, optional): Output format (telegram, etc.)

**Outputs:**
- MEDIA: path to audio file

**Examples:**
```
tts text: "Hello world"
```

**Pitfalls:**
- Requires TTS service configured
- Limited voice options
- May not support all languages

**Best Practices:**
- Keep text concise
- Use for storytelling, not long content
