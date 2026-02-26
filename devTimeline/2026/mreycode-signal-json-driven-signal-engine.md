# 2026: Mreycode-Signal — My First Vibecoding Project

## Mreycode-Signal (Open Source)

**Website:** https://mreycode-signal.vercel.app  
**Type:** Open Source Project  
**Concept:** JSON → Real-Time Visualization Engine  

This was my first real **vibecoding** project.

No manual UI dragging.  
No overthinking architecture for weeks.  
No heavy back-and-forth iterations.

Just a **proper prompt**, clear thinking, and execution — built using Google Antigravity IDE.

And it worked.

---

## The Idea

I wanted a system where:

> You define a JSON config →  
> It fetches data from an API →  
> It visualizes it automatically.

Simple. Flexible. Reusable.

Not hardcoded dashboards.  
Not tightly coupled charts.

A **Signal Engine** powered entirely by configuration.

---

## The Core Concept: JSON-Driven Widgets

Each widget is defined by a structured JSON object.

Example:

```json
{
    "id": "philippines-population",
    "type": "stat",
    "label": "Philippines Population",
    "api": "https://restcountries.com/v3.1/name/philippines",
    "method": "GET",
    "responsePath": "0.population",
    "size": "sm",
    "description": "Current population of the Philippines",
    "refreshInterval": 3600000,
    "sourceUrl": "https://restcountries.com/v3.1/name/philippines"
}
```

From that single configuration:

- It calls the API  
- Extracts the value using `responsePath`  
- Renders a visual stat component  
- Auto-refreshes based on interval  
- Displays the source for transparency  

No extra wiring needed.

Just JSON → Signal → UI.

---

## Why I Built This

I’ve worked with dashboards, analytics, APIs, and admin panels.

Most systems:
- Hardcode API calls  
- Hardcode layouts  
- Hardcode transformations  

I wanted something:
- Modular  
- Configurable  
- Reusable across projects  
- Clean enough to scale  

Something that feels like:
> Infrastructure for micro-analytics widgets.

---

## What I Learned

This project taught me:

- How powerful structured configuration can be  
- How to design systems that are not tightly coupled  
- How to trust a well-written prompt and move fast  
- How to think in “engines” instead of “features”  

It also proved something to me:

You don’t always need massive complexity to build something powerful.

Sometimes you just need:
- Clear architecture  
- Clean contracts (JSON schema)  
- And confidence to ship  

---

## Why It Matters to Me

This wasn’t just another project.

This was my first time building something in a **vibecoding style** —  
minimal friction, maximum clarity.

And it’s open source.

Because tools like this shouldn’t be locked away.

---

Mreycode-Signal is not just a widget system.

It’s a small experiment in how flexible systems should be built.