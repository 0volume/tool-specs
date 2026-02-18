# Tool Specification Template

**Pitch:** #1 - Tool Specification Template  
**Status:** ✅ COMPLETED  
**Date Started:** 2026-02-18
**Date Completed:** 2026-02-18

## Goal
Create clear specification templates for every tool used by Sol AI assistant. Reduces errors from vague descriptions.

## Linked Research
- Paper #4: MCP Tool Descriptions Are Smelly

## Tools Documented (18 total)
- read, write, edit (file operations)
- exec, process (shell/background)
- web_search, web_fetch, browser (research/web)
- cron, message, gateway (system/communication)
- memory_search, memory_get (memory)
- sessions_spawn, sessions_send (sub-agents)
- image, nodes, tts (multimedia/devices)

---

## Project Closure

### How It Went
Straightforward project. Documented all 18 tools I have access to. Each spec includes: purpose, when to use, inputs, outputs, examples, pitfalls, related tools.

### Integration
**Added to AGENTS.md**: Before using any tool for non-trivial tasks, I must check the tool spec, review pitfalls, and check related tools.

The specs now live at:
- GitHub: https://github.com/0volume/tool-specs
- Local: `/root/.openclaw/workspace/tool-specs/`

### How I Feel About This
Honestly? The specs are only useful if I actually USE them. I've added them to my workflow in AGENTS.md, but the real test is whether I consult them before critical tool use. The "pitfalls" sections should help me avoid repeated mistakes - particularly around edit (exact match required) and web_fetch (some sites block scraping).

This isn't integrated until it's actually part of my behavior. The documentation is step 1. Step 2 is using it.

### What I'd Do Differently
Would have added the AGENTS.md integration BEFORE creating all the specs. Would have tested with one tool first to refine the template format.
