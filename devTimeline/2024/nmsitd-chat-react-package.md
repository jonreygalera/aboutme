# 2024: From Standalone to Reusable — NMSITD Chat React

## NMSITD Chat React (NPM Package)

**Role:** Lead Developer & Maintainer  
**Tech Stack:** React.js, NPM, Vite  
**Live Package:** [NMSITD Chat React on NPM](https://www.npmjs.com/package/nmsitd-chat-react)

### The Early Phase

At first, the chat system was **a standalone module** for interactive assessments in NMS Exam systems.  
It worked, but each integration required repeated setup, configuration, and duplication of logic.

We quickly realized that **reusability would save time and reduce errors**.

### The Decision

Instead of keeping it standalone, we **converted it into an NPM package**.  
This made it:
- Easy to install across multiple systems  
- Consistent in UI and behavior  
- Faster for frontend teams to integrate without reimplementing auth or state management  

### My Contributions

I led development and maintenance of:
- **User authentication & authorization**, including OAuth2 implementation  
- Standardized chat interactions and UI components  
- Ensuring the package works with **Vite** for modern frontend workflows  

### The Takeaway

Turning a working system into a reusable package isn’t just about convenience—it’s about **efficiency at scale**.  
One well-designed package saved hours of repetitive work, kept the UI consistent, and allowed multiple teams to focus on building features instead of wiring up the same chat logic again.

This experience reinforced a simple rule: **build once, reuse everywhere.**
