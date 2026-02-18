## gateway
**Purpose:** Restart, apply config, or update the OpenClaw gateway

**When to use:**
- Applying configuration changes
- Restarting after updates
- Checking config schema

**Inputs:**
- `action` (string, required): restart/config.get/config.schema/config.apply/update.run

**Outputs:**
- Action result or config data

**Examples:**
```
gateway action: "config.get"
gateway action: "restart"
```

**Pitfalls:**
- Restart disconnects current session
- Config changes may break things
- Update can be time-consuming

**Best Practices:**
- Use config.get before applying
- Test changes in safe way
- Keep backup of working config
