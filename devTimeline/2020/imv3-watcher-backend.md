# 2020: The Silent Guardian

## IMv3 Watcher

**Role:** Main Developer  
**Tech Stack:** Node.js, Express.js

### The Problem

Messages were getting "stuck." In a complex distributed system, sometimes a message would be sent but not delivered, or delivered but not acknowledged. We had "ghost" conversations.

### The Watcher

I built a backend service whose only job was to **watch**.
It monitored conversation states in real-time. If a message hung in limbo, the Watcher flagged it.
This project taught me about **observability**. You can't fix what you can't see.
The Watcher gave us eyes on the system's health.
