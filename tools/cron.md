## cron
**Purpose:** Schedule automated tasks (cron jobs) and send wake events

**When to use:**
- Scheduling periodic research
- Setting up reminders
- Automating routine checks

**Inputs:**
- `action` (string, required): status/list/add/update/remove/run/wake
- `job` (object, optional): Job definition for add
- `jobId` (string, optional): Job ID for other actions
- `schedule` (object, optional): when to run (at/every/cron)

**Outputs:**
- Confirmation or job list

**Examples:**
```
cron action: "list"
cron action: "add", job: {"name": "research", "schedule": {...}, ...}
```

**Pitfalls:**
- Schedule times are UTC by default
- Jobs run in isolated sessions - no access to main session context
- 90-second timeout limit on jobs
- Complex schedules can be hard to debug

**Best Practices:**
- Use simple schedules initially
- Test with "run" before relying on schedule
- Keep jobs focused and quick

**Related tools:**
- message (for sending results)
