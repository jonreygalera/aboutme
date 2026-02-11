# 2023: Solve It Once, Not Five Times

## NMS Laravel Utility (Composer Package)

**Role:** Lead Developer  
**Tech Stack:** PHP, Laravel, Composer

### The Pattern I Couldn’t Ignore

Every system had the same problem.
Different response formats. Different error codes. Different ways of saying the same thing.

It wasn’t broken—but it was noisy.
And it slowed everyone down.

Every new API meant:
- Re-explaining response structures
- Rewriting validation errors
- Re-deciding status codes

That repetition felt wrong.

### The Decision

Instead of fixing it project by project, I decided to **fix it at the source**.
I built an internal **Laravel Composer package** that standardized:
- API response structures
- Error formats and codes
- Common backend conventions

One package. One way of doing things.

### Why a Package?

Before this, changes had to be copied manually across repositories.
That was slow and error-prone.

With a Composer package:
- Improvements could be rolled out everywhere
- Bug fixes lived in one place
- New projects started with sane defaults

Consistency stopped being optional.

### The Impact

Teams moved faster.
APIs became predictable.
Reviews focused on logic—not formatting.

Most importantly, developers stopped arguing about response shapes and got back to solving real problems.

### Lesson Learned

Internal tools don’t look impressive on a demo slide.
But they quietly multiply a team’s effectiveness.

This package didn’t just clean up code—it reduced friction across every system that used it.
And that kind of leverage is worth building.
