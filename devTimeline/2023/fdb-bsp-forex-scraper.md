# 2023: Oops, the Scraper Broke

## Finance Dashboard (FDB) — BSP Forex Scraper

**Role:** Maintainer  
**Tech Stack:** PHP

### The Moment It Failed

One day, finance data stopped updating.
No errors. No warnings. Just… missing numbers.

The old scraper was no longer working.
Websites change. HTML shifts. PDFs move.
And suddenly, the daily forex report everyone relied on was gone.

### Fixing What Couldn’t Wait

This wasn’t a “let’s refactor later” situation.
Finance needed the data back—fast.

So I rebuilt the scraper from scratch using **PHP**.
Instead of relying on brittle page structures, I focused on pulling **Forex PDF files directly from the Bangko Sentral ng Pilipinas (BSP)** website and processing them reliably.

### What the Script Did

- Automatically downloaded daily BSP Forex PDFs  
- Parsed and extracted the required exchange rate data  
- Updated FDB with clean, consistent values  

Simple on paper.
Careful in execution.

### The Result

Scraping failures dropped.
Daily forex updates became reliable again.
And finance teams stopped asking, *“Why is today’s rate missing?”*

### Takeaway

Scrapers don’t fail loudly.
They fail quietly—and that’s what makes them dangerous.

This reminded me that maintenance work isn’t just fixing bugs.
Sometimes, it’s rebuilding invisible systems that people assume will *always* work.
