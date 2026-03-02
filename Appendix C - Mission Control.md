A mega-prompt for building a full-featured mission control dashboard. This creates a Next.js 15 app with Convex backend, Tailwind CSS, Framer Motion animations, and ShadCN components.

This is an advanced setup. Only use this once you have a working OpenClaw with several active workflows.

---

## The Prompt

Send this to your OpenClaw:

```text
Build me a mission control dashboard called "Jarvis". Stack: Next.js 15 (App Router) + Convex + Tailwind CSS v4 + Framer Motion + ShadCN UI components.

Dark mode only. Responsive. Auto-refresh data every 15 seconds. Host locally.

## Pages

### 1. Home — System Overview
- Agent status cards (online/offline, current task, model, uptime)
- Cron job health (next fire times, last success/fail)
- Quick stats: today's API cost, messages sent, tasks completed
- System health: CPU, memory, disk usage
- Recent activity feed (last 20 actions)
- Secrets health: last rotation dates, any expired keys

### 2. Ops — Tasks & Calendar
- Kanban board: To-do / In Progress / Done / Blocked
- Task creation with priority (P0-P3), deadline, assignee
- Calendar view of scheduled tasks and cron jobs
- Overdue task alerts

### 3. Agents — Multi-Agent Dashboard
- Agent cards: name, role, model, status, current task
- Session history per agent
- Inter-agent message log
- Shared context file browser
- Agent-channel bindings (which agent handles which channel/topic)
- Binding management (bind/unbind from dashboard)

### 4. Chat — Conversation Interface
- Send messages to any agent
- View conversation history
- Quick action buttons (new session, switch agent, approve/reject)

### 5. Content — Content Pipeline
- Pipeline kanban: Research / Draft / Review / Approved / Published
- Draft preview with approve/reject/edit buttons
- Publishing queue with scheduled dates
- Performance metrics for published content

### 6. Knowledge — Searchable Knowledge Base
- Full-text search across workspace/knowledge/
- Tag filtering
- Recent additions
- Source links

### 7. CRM — Relationships
- Contact list with last contact date
- Follow-up reminders
- Interaction history per contact
- Reconnect suggestions

### 8. Analytics — Cost & Performance
- API cost breakdown by provider, model, task type
- Daily/weekly/monthly spend charts
- Token usage trends
- Per-workflow cost analysis
- Budget vs actual
- Secrets rotation status (last rotated date per key)

## Data Source
All data reads from workspace files via API routes. Convex handles real-time sync.

## Design
- Clean, minimal, dark UI
- Card-based layouts
- Smooth Framer Motion transitions between pages
- Toast notifications for alerts
- Command palette (Cmd+K) for quick navigation
```

---

## Notes

- This is a starting point. Iterate on it — add pages as your workflows grow.
- The prompt is intentionally detailed so the agent builds something complete on the first pass.
- If you don't need all 8 pages, remove the ones you don't need before sending.
- You can swap the tech stack (e.g., use Supabase instead of Convex, or plain React instead of Next.js).
