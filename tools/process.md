## process
**Purpose:** Manage background exec sessions

**When to use:**
- Interacting with long-running CLI tools
- Tmux/screen sessions
- Background tasks

**Inputs:**
- `action` (string, required): list/poll/log/write/send-keys/kill
- `sessionId` (string, optional): Session to manage
- `data` (string, optional): Data to write

**Outputs:**
- Session output or status

**Examples:**
```
process action: "list"
process action: "write", sessionId: "abc", data: "command\n"
```

**Pitfalls:**
- Need session ID from exec with background:true
- Can leave orphaned processes
- May timeout

**Best Practices:**
- Always kill sessions when done
- Use timeout parameter
- Check status with poll

**Related tools:**
- exec (create background sessions)
