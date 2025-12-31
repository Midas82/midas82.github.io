# PWA Portfolio Guidelines

## Purpose
`midas82.github.io` is the **official showcase** for all Midas Digital Solutions PWAs. This site is for sharing apps with friends, family, and testers who can install them on any device.

## Rules for Adding Apps

### 1. **PWA-Only Policy**
- **ONLY** Progressive Web Apps (PWAs) go on the portfolio
- All apps **MUST** be installable on any device
- All apps **MUST** work offline with local storage
- CLI tools, desktop apps, or server-only projects do NOT go here

### 2. **Required Files for PWA**
Every app directory must include:
- `manifest.json` with:
  - `display: "standalone"`
  - App icons (192x192, 512x512)
  - `start_url` configured
- Service worker for offline caching
- `index.html` with manifest link
- `DEPLOYMENT.md` documenting:
  - Live URL
  - Portfolio integration
  - Auto-deployment process
  - Development to-do list

### 3. **Deployment Process**
1. Create GitHub repo: `Midas82/<app-name>`
2. Set up GitHub Actions workflow (`.github/workflows/deploy.yml`)
3. Configure GitHub Pages source: "GitHub Actions"
4. Test at `https://midas82.github.io/<app-name>/`
5. Add card to portfolio `index.html`

### 4. **Portfolio Card Template**
```html
<a href="./<app-name>/" class="card app-card">
    <div class="app-icon">🎯</div>
    <div class="app-name">App Name</div>
    <p class="app-desc">Brief description (1-2 sentences max)</p>
    <span class="badge">PWA</span>
</a>
```

### 5. **Card Requirements**
- **Icon**: Use relevant emoji (single character)
- **Name**: App's display name
- **Description**: 1-2 sentences explaining what it does
- **Badge**: Always "PWA"

## Current PWAs

### Live
- ⚡ **Life Guardrail** - `/life-guardrail/` - Alarm & timer system
- 🎰 **Maverick Arcade** - `/maverick_arcade/` - Task wheel spinner

### To Convert
- 🎣 **Py-Line Fishing** - Currently CLI, needs web version

## Future Apps Checklist

Before adding ANY new app:
- [ ] Is it a PWA? (Must be yes)
- [ ] Does it have a manifest.json?
- [ ] Does it work offline?
- [ ] Can it be installed?
- [ ] Is it deployed to `midas82.github.io/<app-name>/`?
- [ ] Is the card added to portfolio?

## Testing Checklist

Before going live:
1. Install on desktop (Chrome/Edge)
2. Install on Android
3. Test offline mode
4. Verify local storage works
5. Share link with tester

---

**Last Updated:** 2025-12-30  
**Maintained By:** Midas + AI
