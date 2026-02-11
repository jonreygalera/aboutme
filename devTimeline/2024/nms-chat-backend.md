# 2024: Making Chats Work Behind the Scenes

## NMS Chat Backend

**Role:** Lead Developer  
**Tech Stack:** Laravel, PHP, MySQL, Redis

### The Challenge

Chats feel instant.
Users expect messages to appear immediately.
But behind every real-time conversation is a backend that has to handle scaling, delivery, and reliability.

The NMS Chat backend was powering **NMS Exam systems**, where timely communication wasn’t just convenient—it was critical.

### How It Worked

The system required a **conversation key** to allow clients to connect and participate.  
It **stored and managed messages**, tracked conversation state, and handled **clients/participants** reliably.  
Every message, every participant, and every key had to be accounted for—otherwise the system would break silently.

### My Role

As lead developer, I ensured:

- Real-time message delivery with **Redis-powered queues**
- MySQL records for conversation history and auditing
- Secure management of conversation keys and participants
- Reliable system operation under multiple concurrent users

Even small mistakes could cause delays or lost messages.

### Lessons Learned

This project reminded me that **infrastructure is invisible when it works**.
No one notices a chat backend unless it fails.
Making messaging reliable taught me patience, careful design, and the importance of planning for scale.
