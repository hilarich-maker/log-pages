# log-pages

Public support and privacy pages for the Log app portfolio.

This folder is a **copy-ready draft** of the public GitHub Pages repo named `log-pages`.

It is content only. It does not affect Flutter app code, signing, versions, or product IDs.

## File structure

```text
log-pages/
  index.html
  README.md
  homelog/
    privacy-policy.html
    support.html
```

Future apps may later add folders such as:

```text
vehiclelog/
petlog/
plantlog/
```

Do not invent those pages until each app is ready for store listing.

## Placeholders to replace before publishing

Search for these exact strings:

| Placeholder | Replace with |
| --- | --- |
| `SUPPORT_EMAIL_HERE` | Real support email |
| `DEVELOPER_NAME_HERE` | Real developer / seller name |
| `EFFECTIVE_DATE_HERE` | Privacy Policy publication date |
| `GITHUB_ACCOUNT_HERE` | GitHub account that will host `log-pages` |

Do not invent a company name or email.

## Expected final URLs

After GitHub Pages is enabled on the public `log-pages` repo:

```text
https://GITHUB_ACCOUNT_HERE.github.io/log-pages/
https://GITHUB_ACCOUNT_HERE.github.io/log-pages/homelog/privacy-policy.html
https://GITHUB_ACCOUNT_HERE.github.io/log-pages/homelog/support.html
```

Use the HomeLog Privacy Policy and Support URLs in:

- App Store Connect → Privacy Policy URL / Support URL
- Google Play Console → Privacy policy / Support

## How to publish (separate public repo)

1. Create a **public** GitHub repository named `log-pages` under `GITHUB_ACCOUNT_HERE`.
2. Copy the contents of this folder into that repo root (keep `index.html`, `README.md`, and `homelog/`).
3. Replace all placeholders in the HTML files.
4. On GitHub: **Settings → Pages**
5. Source: **Deploy from a branch**
6. Branch: `main` (or default), folder: `/` (root)
7. Save, wait for deploy, then open the three URLs above and verify they load on mobile.
8. Paste the live Privacy Policy and Support URLs into the store consoles.

Do **not** publish these pages from the HomeLog app repo `/docs` folder.

## Checklist before store console use

- [ ] Replaced `SUPPORT_EMAIL_HERE`
- [ ] Replaced `DEVELOPER_NAME_HERE`
- [ ] Replaced `EFFECTIVE_DATE_HERE`
- [ ] Replaced `GITHUB_ACCOUNT_HERE` in all URL links
- [ ] Public `log-pages` repo created and Pages enabled from repo root
- [ ] Live HTTPS URLs open correctly on mobile
- [ ] Confirmed pages still match HomeLog v1:
  - local-only storage
  - no account / no login
  - no HomeLog backend / no cloud sync
  - no HomeLog analytics / tracking SDKs
  - attachments on device
  - local reminder notifications
  - Backup / Export / Restore are Premium and user-controlled
  - Apple / Google handle one-time Premium unlock
  - no AI / OCR / image recognition
  - no camera / photos currently
  - uninstall removes on-device app data; outside copies are separate
- [ ] Pasted Privacy Policy URL into App Store Connect and Google Play Console
- [ ] Pasted Support URL into App Store Connect and Google Play Console

## HomeLog v1 facts these pages assume

- Local-first / offline-first
- No backend, no account, no cloud sync
- No analytics / tracking by HomeLog
- Documents/files attachments stored on device
- Local notifications for reminders
- Backup / export / restore are Premium and user-controlled
- Premium one-time unlock via Apple / Google (`homelog_premium_unlock`)
- No AI, OCR, image recognition, or automatic enrichment
- Camera / photos not currently used
- No cloud backup
- No notification deep links claimed
