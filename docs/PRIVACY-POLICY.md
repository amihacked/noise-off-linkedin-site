---
layout: default
title: Privacy Policy
---

# Privacy Policy — NoiseOff for LinkedIn

**Effective date:** 2026-03-23
**Last updated:** 2026-03-23

---

## Summary

NoiseOff for LinkedIn does not collect, transmit, or store any personal data. The extension runs entirely within your browser — no data ever leaves your device.

---

## What data we collect

**None.** NoiseOff does not collect any data of any kind.

- No browsing history
- No personal information
- No usage analytics
- No telemetry
- No crash reports
- No cookies or tracking pixels

---

## How the extension works

### Settings storage

Your filter preferences (enabled filters, allowed language list) are stored using `chrome.storage.sync`, a browser-provided API. This data syncs across your devices via your browser account (Google account for Chrome). NoiseOff has no access to your browser account and does not control this sync — it is handled entirely by the browser.

### Language detection

Post language is detected using two methods, both fully local:

1. **`chrome.i18n.detectLanguage()`** — a built-in browser API that runs entirely on your device.
2. **Unicode script heuristic** — a fallback that analyses character ranges (Greek, Cyrillic, Arabic, CJK, Latin) without any network requests.

No post text is ever sent to any server or third-party service.

### LinkedIn feed interaction

NoiseOff reads the visible text content of LinkedIn feed posts to determine their language. It does not:

- Access your LinkedIn account credentials
- Read your LinkedIn messages or notifications
- Modify any LinkedIn data
- Send any data to LinkedIn's servers
- Interact with LinkedIn's API

### "Show anyway" dismissals

When you click "Show anyway" on a collapsed post, the dismissal is session-only and stored in the page's DOM. It is not persisted to disk and is lost when you navigate away or refresh the page.

---

## Network requests

**NoiseOff makes zero network requests.** The extension contains no code that initiates HTTP requests, WebSocket connections, or any other form of network communication. You can verify this in your browser's DevTools Network tab.

---

## Permissions used

| Permission | Purpose |
|---|---|
| `storage` | Save your filter settings (language list, toggle states) |
| `host_permissions: linkedin.com` | Run the content script on LinkedIn pages to filter the feed |

No other permissions are requested or used.

---

## Third-party services

NoiseOff uses no third-party services, libraries, SDKs, or analytics platforms. The extension is built with vanilla JavaScript and has zero external dependencies.

---

## Data sharing

NoiseOff does not share any data with anyone because it does not collect any data.

---

## Children's privacy

NoiseOff does not knowingly collect any information from anyone, including children under 13 years of age.

---

## GDPR compliance

NoiseOff is GDPR compliant by design. Since no personal data is collected, processed, or stored, there is no data to protect, export, or delete. No consent is required because no processing of personal data occurs.

---

## Changes to this policy

If this privacy policy is updated, the changes will be reflected in this document with an updated "Last updated" date. Significant changes will be noted in the CHANGELOG.

---

## Contact

For questions about this privacy policy:

**Email:** privacy@amihacked.com
**GitHub:** https://github.com/amihacked/noise-off-linkedin

---

## Governing law

This privacy policy is governed by the laws of the European Union.
