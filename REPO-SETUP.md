# Repo Setup: anhafdev/reverse-engineering-automation

Delete this file before pushing. It's only your checklist.

## 1. Title (repo name)
`reverse-engineering-automation`
Transfer the repo from algoanhaf (Settings → Transfer ownership → anhafdev) and keep this exact name. Stars carry over, and old links redirect.

## 2. Description (About box)
```
API reverse engineering & automation: authorized private API analysis, OpenAPI docs, Python SDKs, web scraping, Playwright automation and Telegram bots. By F. ANHAF DEV.
```

Website: `https://anhaf.dev`

## 3. Tags (Topics, 20 max)
```
reverse-engineering api-reverse-engineering private-api api-integration openapi python-sdk web-scraping data-extraction browser-automation playwright mitmproxy frida python-automation telegram-bot aiogram fastapi api-security automation-services freelance-developer python
```

## 4. Image
- **README header:** `assets/header.svg` is animated and already linked in the README.
- **Social preview:** Settings → General → Social preview → upload `assets/social-preview.png` (1280×640). This is the card that shows when the link is shared on Telegram, X, LinkedIn and Upwork.

## 5. Build
`.github/workflows/build.yml` runs ruff (Python lint) and a link check on every push. The **build** badge in the README goes green after the first run.

## 6. Push (as yourself only)
```bash
git config user.name "F. ANHAF DEV"
git config user.email "founder@anhaf.dev"
git add .
git commit -m "docs: rebuild as flagship service page with header, build and license"
git push origin main
```

Then set the description and topics in one go:
```bash
gh repo edit anhafdev/reverse-engineering-automation \
  --description "API reverse engineering & automation: authorized private API analysis, OpenAPI docs, Python SDKs, web scraping, Playwright automation and Telegram bots. By F. ANHAF DEV." \
  --homepage "https://anhaf.dev" \
  --add-topic reverse-engineering,api-reverse-engineering,private-api,api-integration,openapi,python-sdk,web-scraping,data-extraction,browser-automation,playwright,mitmproxy,frida,python-automation,telegram-bot,aiogram,fastapi,api-security,automation-services,freelance-developer,python
```

## 7. After push
- [ ] Fill in the `[ADD]` rows in **Showcase** with real past orders (no client names, no fake numbers)
- [ ] Pin the repo first on your profile
- [ ] Create release `v1.0.0`
- [ ] Update `examples/README.md` statuses as you publish each demo
