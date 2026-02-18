## message
**Purpose:** Send messages via configured channels (WhatsApp, Discord, Telegram, Signal, etc.)

**When to use:**
- Sending notifications to D
- Proactive updates
- Sending to specific channels

**Inputs:**
- `action` (string, required): send/broadcast/react/poll
- `channel` (string, optional): whatsapp/telegram/discord/signal
- `message` (string, required for send): Message text
- `target` (string, optional): Recipient

**Outputs:**
- Message send confirmation with ID

**Examples:**
```
message action: "send", channel: "whatsapp", message: "Update complete", target: "+447535346950"
```

**Pitfalls:**
- Requires channel to be configured
- May have rate limits
- Some features (inline buttons) require specific config

**Best Practices:**
- Keep messages concise
- Use appropriate channel for urgency
- Don't spam - respect quiet hours

**Related tools:**
- cron (for scheduled messaging)
