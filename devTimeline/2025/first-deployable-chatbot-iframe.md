# 2025: First Deployable Chatbot Iframe — Plug & Play AI Widget

## Script-Based Chatbot Embed System

**Role:** Fullstack Developer  
**Tech Stack:** ReactJs, JavaScript (DOM), Iframe, Backend API Integration, 3rd Party APIs  

### The Idea

In 2025, I created my first **deployable chatbot widget**.

Not just a chatbot UI —  
but a script-based iframe embed system that can be deployed to any website using a simple `<script>` tag with query parameters like `agentName`.

Just drop the script into any website, and the chatbot appears automatically.  
It was **implemented on this website**: [https://newmediaservices.com.au/](https://newmediaservices.com.au/)

### What It Does

- Dynamically injects a floating chat button  
- Loads the chatbot using a DOM-created iframe  
- Supports parameters such as:
  - `agentName`
  - `cname` (custom chatbot name for UI)
- Securely passes the parent domain to the backend
- Smooth open/close toggle animations  
- Fully responsive (mobile full-screen mode)  
- Cross-window communication using `window.postMessage`  
- Loading states and clean UI transitions  
- Maintains guest conversation sessions using **cookies**

### Session Handling

One important decision:  
I chose **cookies instead of localStorage** to persist guest conversations.

Why cookies instead of localStorage?

- Keeps session tied to the domain properly  
- Allows backend-controlled session validation  
- Avoids exposing sensitive conversation identifiers directly in browser storage  
- Makes conversation recovery cleaner and more secure  
- Enables **analytics tracking**, like monitoring usage across multiple sessions, without polluting the client’s localStorage  

This allowed guest users to:
- Close the tab  
- Reopen the site  
- Continue the same conversation seamlessly  

Without relying on localStorage hacks.

### The Technical Side

The script:

- Prevents double initialization using a global window guard  
- Extracts configuration from `document.currentScript`  
- Dynamically injects scoped CSS styles  
- Lazily creates and mounts the iframe only when needed  
- Uses `postMessage` for controlled communication between iframe and parent  
- Handles mobile UX properly by locking background scroll  
- Syncs session state via cookies for persistent guest conversations  

This wasn’t just embedding an iframe.  
It was building a reusable, deployable chatbot infrastructure.

### Why This Was Important

This project shifted my thinking.

I wasn’t just building a chatbot anymore.  
I was building something that could be embedded into **any website**.

It introduced me to distribution thinking:
- Not just a standalone app  
- Not just an API  
- But a pluggable system  

A small script.  
A big capability.  

And this was my first version.