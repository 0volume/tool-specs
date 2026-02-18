## exec
**Purpose:** Execute shell commands on the host system

**When to use:**
- Running scripts, git commands
- System operations
- Anything requiring command-line tools

**Inputs:**
- `command` (string, required): Shell command to execute
- `timeout` (number, optional): Seconds before killing process
- `background` (boolean, optional): Run in background
- `pty` (boolean, optional): Use pseudo-terminal for TTY-required CLIs

**Outputs:**
- Command output (stdout/stderr)

**Examples:**
```
exec command: "ls -la"
exec command: "python3 script.py", timeout: 30
```

**Pitfalls:**
- **POTENTIALLY DESTRUCTIVE**: Can run rm, delete files, etc.
- Timeout may not work for all commands
- Background processes may be orphaned
- Output can be large - consider timeout

**Best Practices:**
- Always confirm destructive commands
- Use timeout for long-running commands
- Prefer specific over general commands

**Related tools:**
- process (manage background sessions)
