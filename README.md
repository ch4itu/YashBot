# 🟣 Universal Agent (Decentralized AI System)

> "Control your computer from anywhere using Blockchain and AI."

## 🚀 Overview
**Universal Agent** is a secure, serverless, and completely decentralized AI assistant that lives in your browser. It uses the **Algorand Blockchain** as a sync server, allowing you to send encrypted commands from your phone to your PC without needing to rent a VPS, install Node.js, or configure firewalls.

**Zero Dev Hell:** Runs natively in Chrome/Edge using standard HTML5.

### ✨ Key Features
* **🌍 Infinite Range:** Works from anywhere in the world.
* **🔒 Military-Grade Encryption:** All commands are AES-GCM encrypted. Even the public blockchain cannot see your data.
* **🧠 Persistent Memory:** The Agent remembers your name, preferences, and projects in `memory.txt`.
* **🗣️ Voice Control:** Speak commands to your phone; your PC speaks back when done.
* **⏰ Autonomy:** Schedule tasks (e.g., "Check crypto prices every day at 9 AM") and the Agent executes them automatically.
* **📂 File System Access:** Can Read, Write, and Analyze files on your local hard drive.

---

## 🛠️ Setup Guide

### Part 1: The PC Agent (The Brain)
1.  Download `agent.html`.
2.  Create a folder on your PC (e.g., `Documents/MyAI`).
3.  Move `agent.html` into that folder.
4.  Open `agent.html` in **Google Chrome** or **Edge**.
5.  **Configuration:**
    * **Network:** Select `Testnet` (Free) or `Mainnet`.
    * **Wallet Address:** Enter your main Algorand Address.
    * **Encryption Password:** Create a strong password (e.g., `XenoProject2026`).
    * **API Key:** Enter your Gemini (Free) or OpenAI Key.
6.  Click **INITIALIZE SYSTEM**.
    * Allow the browser to access the folder.

### Part 2: The Phone Remote (The Commander)
1.  Download `sender.html`.
2.  **Hosting:** You must host this file securely so your phone can access it.
    * *Easy Option:* Upload it to a private GitHub Gist or GitHub Pages.
    * *Note:* It requires HTTPS for Voice features to work.
3.  Open the link on your Android Phone (Chrome).
4.  **Configuration:**
    * **Network:** Must match the PC (Testnet/Mainnet).
    * **Target Address:** Paste your PC's Wallet Address.
    * **Sender Mnemonic:** Create a **Burner Wallet** (New Pera Algo account), get 10 Free Testnet Algos, and paste the 25-word mnemonic here.
    * **Encryption Password:** Must match the PC password exactly.
5.  Click **Save & Close**.

---

## 🎮 How to Use

### 1. Basic Commands
Type or Speak these commands into your Phone:
* `Write a python script to calculate Fibonacci numbers.`
* `Create a cyberpunk style HTML landing page.`
* `Analyze {{data.csv}} and summarize the trends.` (Make sure data.csv is in the folder).

### 2. Memory Commands
* `Remember that I am building a game called Xeno Survivor.`
* `Update memory: My preferred coding style is Functional JavaScript.`

### 3. Scheduling
* `Create a schedule to run "Check system logs" every day at 08:00.`
    * *Result:* Creates `schedule.json` and runs automatically.

---

## ❓ Troubleshooting

**Q: The Agent isn't responding.**
* Check if both devices are on the same Network (Testnet vs Mainnet).
* Check if the **Encryption Password** matches exactly.
* Ensure the PC browser tab is open and active (not sleeping).

**Q: Voice Input isn't working.**
* Make sure `sender.html` is served over **HTTPS** (GitHub Pages works best).
* Use Google Chrome on Android.

**Q: Is my mnemonic safe?**
* Your mnemonic is stored in your phone's local browser storage (`localStorage`). It is never sent to any server. However, always use a **Burner Wallet** with small funds, never your main savings wallet.
