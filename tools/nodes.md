## nodes
**Purpose:** Discover and control paired devices (phones, computers)

**When to use:**
- Taking screenshots
- Running commands on devices
- Getting location
- Camera access

**Inputs:**
- `action` (string, required): status/describe/notify/camera_snap/screen_record/run
- `node` (string, optional): Specific device ID
- `command` (array, optional): Commands to run

**Outputs:**
- Action result or data

**Examples:**
```
nodes action: "status"
nodes action: "camera_snap", node: "my-phone"
nodes action: "run", command: ["ls", "-la"], node: "my-phone"
```

**Pitfalls:**
- Requires paired devices
- Some actions need permissions
- Can be slow

**Best Practices:**
- Check node status first
- Be specific about which node
