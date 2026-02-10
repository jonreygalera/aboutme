# 2021: Scaling Up

## Loop Moderation v2

**Role:** Co-Lead Developer  
**Tech Stack:** Laravel, Node.js, Socket.io, React.js

### The Context

Version 1 worked. Version 2 had to **fly**.
We weren't just moderating text anymore; we were handling a massive influx of requests.

### The Architecture

We introduced:

1.  **Queues:** To handle bursts of traffic without crashing.
2.  **Retry Policies:** because third-party APIs _will_ fail, and our system needs to be resilient enough to try again.

This project was a masterclass in **system design**. We moved from "making it work" to "making it unbreakable."
