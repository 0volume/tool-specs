## sessions_spawn
**Purpose:** Spawn a background sub-agent in an isolated session

**When to use:**
- Delegating focused tasks
- Parallel processing
- Research sub-tasks

**Inputs:**
- `task` (string, required): What the sub-agent should do
- `agentId` (string, optional): Which agent to spawn
- `runTimeoutSeconds` (number, optional): Max runtime

**Outputs:**
- Session key for the spawned agent

**Examples:**
```
sessions_spawn task: "Research topic X", agentId: "main"
```

**Pitfalls:**
- Spawns new session - no direct memory access
- Need to use sessions_send to communicate
- Can increase token usage significantly
- Sub-agent may hallucinate if not carefully prompted

**Best Practices:**
- Give very specific instructions
- Review output before using
- Set clear timeout limits

**Related tools:**
- sessions_list (see active sessions)
- sessions_history (get session output)
