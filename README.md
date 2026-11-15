# Automated Office Task Allocation System

A system that **assigns office tasks automatically**. When a new task arrives, it checks who is free and who has the lightest workload, assigns the task to that person, follows up until the task is done, and tracks each person's performance over time.

## What it does

| Feature | How it works |
|---|---|
| Smart assignment | Each new task goes to the available team member with the **lowest current workload**, matched to the type of task |
| Follow-ups | Sends **reminders every hour** until the task is marked complete |
| Task tracking | Stores every task with its status, owner and timestamps |
| Performance tracking | Builds a history per person: tasks completed, time taken and pending work |

## Flow

```
New task ─► check team availability + current load
         ─► assign to the best-fit, least-loaded person
         ─► hourly reminders until done
         ─► mark complete ─► update person's performance history
```

## Tech stack

Python · Flask · SQLite

## Why it helps

- No manual task assignment, and work is spread evenly
- Fewer forgotten tasks, thanks to automatic follow-ups
- Managers see each person's workload and performance in one place

---

*Source code is not public. Available on request.*
