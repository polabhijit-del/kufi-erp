# KUFI ERP

A browser-based CRM & ERP system. Accessible from any device — phone, tablet, or laptop — via GitHub Pages.

**Live URL:** `https://<your-username>.github.io/<repo-name>/`

---

## Features
- Sales Activities & Pipeline tracking
- Customer Master with locations & contacts
- Task Dashboard & Review Meeting
- Daily follow-up tracking
- Backup & Restore (JSON export)
- Works offline after first load
- Mobile-friendly (Android, iPad, laptop)

## Data Storage
All data is stored in the **browser's localStorage** on each device.  
To move data between devices: use **Backup → Export JSON** on the source device, then **Backup → Import JSON** on the target device.

## AI Insights (optional)
Requires an Anthropic API key. Enter it once in the app — it is stored only in your browser's localStorage and never sent anywhere except directly to Anthropic.

## Setup — GitHub Pages (one time)

1. Create a new **private** repository on GitHub (recommended: private so your data structure isn't public)
2. Upload all files from this folder
3. Go to **Settings → Pages**
4. Source: **Deploy from a branch** → branch: `main` → folder: `/ (root)`
5. Save — GitHub will show your live URL within ~60 seconds

## Local Server (optional, for LAN access)
```bash
python3 server.py 8765
```
Then open `http://localhost:8765` or `http://<your-local-ip>:8765` from any device on the same WiFi.
