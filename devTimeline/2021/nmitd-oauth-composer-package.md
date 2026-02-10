# 2021: The "Don't Repeat Yourself" Package

## nmitd/oauth (Private Composer Package)

**Role:** Support Lead Developer  
**Tech Stack:** PHP, Composer, Laravel

### The Problem

We had just built the new Accounts system (SSO). Now we had to connect 10 different legacy apps to it.
Copy-pasting the OAuth integration code 10 times sounded like a punishment.

### The Automator

I wrapped the entire integration logic into a **Composer package**.
Instead of writing 500 lines of code for every app, developers just had to run:
`composer require nmitd/oauth`
And add 3 lines of config.

### The Impact

It turned a week of integration work into an afternoon.
It taught me that the best code is the code you write **once** and reuse **everywhere**.
