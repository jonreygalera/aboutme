# 2019: The Deep End (Legacy vs. New)

## Flai

**Role:** Developer  
**Tech Stack:** Kohana, PHP, MySQL, jQuery

### The Story

**Flai** was my crash course in the reality of software development: **Maintenance**.
I had to dig through legacy code (Kohana frameork!) to keep the system alive while simultaneously building advanced new features.

### The "Aha!" Moment

I was tasked with building a **bulk email system**. I thought, _"Easy, loop through users and send."_
**Wrong.**
I hit rate limits. servers stalled. I learned the hard way about:

1.  **Queue implementation** (don't block the main thread!).
2.  **Throttling** (respect the API limits).
3.  **Error Handling** (what happens when 1 out of 10,000 fails?).

This project taught me that "it works" isn't enough. It has to work _at scale_.
