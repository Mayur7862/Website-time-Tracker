# 🕒 Website Time Tracker (Tampermonkey Script)

A lightweight, non-intrusive userscript that tracks how much time you spend on selected websites like YouTube, Reddit, or Twitter — directly in your browser. Designed to help you stay aware of your online habits without being in your face.

## ✨ Features

- 📌 Minimal timer in the bottom-right corner
- ⏱ Tracks active time per session (resets on refresh)
- 🖥 Works on specific sites (YouTube, Reddit, Twitter by default)
- 💡 Easy to modify, fully open source

## 🚀 Installation

1. **Install [Tampermonkey](https://www.tampermonkey.net/)** extension on your browser (Chrome, Firefox, Edge, etc.)
2. Click on `Create a new script` in Tampermonkey dashboard.
3. Replace the default code with the contents of [`tracker.user.js`](./tracker.user.js)
4. Save and you're done! Visit a supported site to see the timer in action.

## 🛠 Customization

You can easily edit the script to:

- 🕸 Add or remove websites by changing the `@match` lines
- 🎨 Modify the timer's look by tweaking the `CSS` styles
- 💾 Add persistent storage (e.g., `localStorage`) to track total time across sessions (future version!)

## 📂 Example Usage

![](./preview.png) <!-- Optional: add a screenshot if you'd like -->

## 📜 Sample Code Snippet

```javascript
timer.textContent = `Time: ${mins}m ${secs}s`;
