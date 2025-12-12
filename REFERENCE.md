# Midas82.github.io - Master Reference

> **Your Website:** https://midas82.github.io

---

## Quick Commands

### Serve locally for testing
```bash
cd /path/to/your/app
python -m http.server 8080
# Open http://localhost:8080
```

### Share to phone via USB (ADB)
```bash
adb devices                          # Check connection
adb reverse tcp:8080 tcp:8080        # Forward port
# On phone: http://localhost:8080
```

### Deploy to GitHub Pages
```bash
cd /run/media/midas/PARKING-GARAGE/PriorityFocusAlarm/midas82.github.io
git add .
git commit -m "Update"
git push
# Live in ~1 minute at https://midas82.github.io
```

---

## Apps Deployed

| App | Local Path | Live URL |
|-----|------------|----------|
| Life Guardrail | `LifeGuardrail_v1/` | [midas82.github.io/life-guardrail](https://midas82.github.io/life-guardrail) |

---

## Session Log

### 2025-12-12
- Added PWA service worker to Life Guardrail (`sw.js`)
- Registered service worker in `index.html`
- Created GitHub Pages website structure
- Built landing page with Midas Standard aesthetics

---

## File Locations

| Purpose | Path |
|---------|------|
| Website Repo | `/run/media/midas/PARKING-GARAGE/PriorityFocusAlarm/midas82.github.io/` |
| Life Guardrail (source) | `/run/media/midas/PARKING-GARAGE/PriorityFocusAlarm/LifeGuardrail_v1/` |
