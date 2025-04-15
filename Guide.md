# Removing Adware and Fake Notifications on macOS Monterey

This guide documents the step-by-step process I followed to help a friend clean adware off their MacBook running macOS Monterey.  
They were receiving fake alert notifications in Safari and experiencing random shutdowns.  
Since I couldn’t access Safari settings in the original user account, I used a workaround and performed the cleanup through a new user account.

> **⚠️ Note:** Before deleting any files or killing processes, always double-check their legitimacy.  
> Misidentifying a system process can cause unexpected issues. When in doubt, use tools like [VirusTotal](https://www.virustotal.com/) or search online for clarification.

---

## ✅ Step 1 – Check for Suspicious Startup Items

Before running any tools, I manually checked for signs of malware by inspecting Launch Agents and Daemons—common hiding spots for persistent malware.

### 📂 Accessing the Library

1. Open `Finder > Go > Home`
2. Click `Go` again, then hold the **Option** key and select `Library`
3. Navigate through these folders and inspect contents:

- `~/Library/LaunchAgents/`
- `/Library/LaunchDaemons/`
- `/Library/StartupItems/` *(obsolete, but worth checking if present)*

> 🕵️ Look for unfamiliar app names, randomized filenames, or recently modified files.  
> If anything looks suspicious, do some research before deleting.

### 🚩 Known Suspicious Files or Common Adware Names

Some file names may vary slightly or be randomized. Watch out for names like:

- `com.pcv.hlpramc.plist`
- `com.adobe.fpsaud.plist` *(fake version, not legit Flash)*
- `com.mcp.agent.plist`
- `com.avickUpd.plist`
- `com.myppes.download.plist`
- `maccleaner.pkg` *(or any “cleaner” tool you didn’t install)*
- `com.3gXJ4sd2.random.plist` *(random strings like this)*

> 📌 Tip: If in doubt, copy the file name and Google it, or upload to [VirusTotal](https://www.virustotal.com/).

---

## ✅ Step 2 – Use Activity Monitor to Spot Suspicious Processes

Activity Monitor gives a live overview of what’s running on the system—essential for identifying rogue processes tied to adware or unnecessary background tasks.

### 🧭 Open Activity Monitor

1. Press `Cmd + Space` to open Spotlight  
2. Type `Activity Monitor` and hit Enter

### 📊 Sort by Resource Usage

- Go to the **CPU** tab → Sort by `% CPU`
- Go to the **Memory** tab → Look for anything with high memory usage

> 👀 Take note of processes with strange names or anything using a lot of resources for no clear reason.

### 🧪 Inspect Unfamiliar Processes

- Right-click the process → `Inspect` or `Sample Process`
- Google suspicious names or scan on [VirusTotal](https://www.virustotal.com/)

> ❗ **Don't kill random processes blindly.** Use VirusTotal for analysis and verification—especially when combined with findings from the next steps.

---

## ✅ Step 3 – Identify Fake Notifications and Browser Hijacking

Once connected to the internet, the user was receiving fake system notifications.

> 💡 Many of these pop-ups are from websites granted notification access—not from macOS itself.

### 🔎 What to Look For

- Spelling mistakes and weird grammar in the notifications  
- Notifications only appear while online  
- Behavior consistent with adware exploiting browser notification permissions

![Example of fake Safari notification with broken grammar and sketchy URL](path-to-image)

---

