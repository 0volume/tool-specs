## sessions_send
**Purpose:** Send a message into another session or sub-agent

**When to use:**
- Communicating with spawned sub-agents
- Sending tasks to other sessions

**Inputs:**
- `sessionKey` (string, required): Target session
- `message` (string, required): Message to send

**Outputs:**
- Confirmation of message delivery

**Examples:**
```
sessions_send sessionKey: "abc123", message: "Your findings?"
```

**Pitfalls:**
- Need correct session key
- Response comes in separate turn
- Can be slow for back-and-forth

**Related tools:**
- sessions_spawn (create sub-agent)
- sessions_history (get conversation)
