# ISC2 CC Trainer

Practice web app for the **ISC2 Certified in Cybersecurity (CC)** exam, updated for the exam outline effective **September 1, 2026**.

**Open it:** https://frankar100.github.io/ssdlc-security-scanner/

## Features

- **384 questions** across the five 2026 domains:
  1. Security Principles (24%)
  2. Security Governance (17.3%)
  3. Identity and Access Management (IAM) Concepts (20%)
  4. Networking and Cloud Security Concepts (21.3%)
  5. Security Operations and Incident Response (17.3%)
- **Smart Practice**: adaptive flashcards; questions you fail come back more often.
- **Review my mistakes** and **practice by domain**.
- **Exam simulation**: 100 items, 2 hours, distributed by the official domain weights, no going back, review at the end.
- **Progress saved automatically** in the browser (localStorage). Use *Export / Import progress* to move it between devices.
- Works on PC and mobile; can be installed as an app (PWA) and works offline.

## Install on your phone

- **Android (Chrome):** open the link → menu ⋮ → *Add to Home screen* / *Install app*.
- **iPhone (Safari):** open the link → Share → *Add to Home Screen*.

## Development notes

- Everything lives in `index.html` (questions in the `QB` array).
- Progress is stored by **question index**: never reorder or delete questions in `QB`; only append new ones at the end.
- When you change files, bump the cache name in `sw.js` so installed apps pick up the update.
