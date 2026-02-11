# 2024: Leadgen — Automating Leads Without Losing Sleep

## Leadgen

**Role:** Co-Lead Backend Developer  
**Tech Stack:** Laravel, Docker, Redis, MySQL  

### The Challenge

Marketing teams were drowning in manual lead collection and follow-ups.
Emails were being sent inconsistently, follow-ups were delayed, and queues sometimes overlapped.  

The system needed to **automate everything** while ensuring **race conditions didn’t break it**.

### My Role

As co-lead for the backend, I handled:
- API development and system integration  
- Backend architecture decisions for queueing and reliability  
- Job queue management with **Redis**, ensuring email sending and follow-ups ran smoothly  

Pausing or stopping the queues at the right time without causing duplicates was tricky, but crucial for accuracy.

### What We Built

Leadgen could:
- Automatically collect leads  
- Send initial emails and follow-ups based on schedules  
- Pause, resume, or stop queues safely without losing track  
- Reduce manual work for marketing teams drastically  

The combination of **Redis queues** and careful backend design made the system reliable and scalable.

### Reflection

Automation isn’t just about reducing clicks—it’s about **trusting the system to act correctly when humans aren’t watching**.  

This project taught me a lot about concurrency, queues, and the subtle challenges of keeping background tasks predictable.
