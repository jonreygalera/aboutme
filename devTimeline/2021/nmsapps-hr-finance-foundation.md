# 2021: Before Features, There Was Infrastructure

## HR & Finance — NMSAPPS (Early Development)

**Role:** Co-Lead (Environment & Setup)  
**Tech Stack:** Laravel, Docker, MySQL, Node.js

### The Unseen Start

Before dashboards, payroll logic, or HR workflows existed, there was a harder question:
**How do we build this the right way from day one?**

This was the start of NMSAPPS HR and Finance.
No users yet. No features to demo.
Just a blank repository and a lot of decisions that would be painful to undo later.

### Owning the Environment

As co-lead, I focused on **environment setup across all stages**—local, staging, and production.
Consistency mattered.
We wanted developers to stop saying, _“It works on my machine.”_

This meant defining:

- Base project structure
- Environment configuration standards
- Containerized setups so onboarding didn’t take days

It wasn’t glamorous work, but it removed friction for everyone who touched the codebase after.

### Why This Phase Mattered

Most systems fail quietly because of weak foundations.
Bad environment setup turns simple changes into risky deployments.
We didn’t want that.

By setting things up properly early, we made it easier to:

- Scale development safely
- Onboard new developers faster
- Build HR and Finance features without fighting the tooling

### Looking Back

No end user ever sees environment setup.
But every bug avoided, every smooth deployment, and every fast onboarding traces back to this phase.

This was one of those moments where I learned:
**good systems start long before the first feature is written.**
