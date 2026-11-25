# FairSplit privacy policy

_Last updated: 26 November 2026_

FairSplit helps people who live or travel together split expenses, share duties and manage their
own money. This page explains what the app stores, where, and who can see it.

## What we store

| Data | Where | Who can see it |
|---|---|---|
| Your name, email and profile picture | Google Firebase (Firestore) | People in your home |
| Shared expenses, payments, groups and duties | Firestore, inside your home | Members of that home, or of that group or 1-on-1 ledger |
| Your personal ledger, budgets, goals and accounts | Firestore, under your account | Only you |
| Photos and voice notes you attach | **Only on phones**, never uploaded | The people the item is shared with, copied phone to phone over Bluetooth or Wi-Fi |
| A tiny blurred preview of attached photos | Firestore | The same people as the photo |

Sign-in uses your Google account through Firebase Authentication. We don't receive your password.
Your profile picture is copied from your Google account the first time, unless you change it. It's
resized and re-encoded on your phone before it's stored.

## What we don't do

- No ads, no tracking, no analytics SDKs, no selling or sharing data.
- No access to your contacts, SMS or location. Bluetooth and nearby-device permissions are used
  only to copy attachments between phones in the same home.

## Security

- Every read and write is checked by Firestore security rules: you can only reach your own homes
  and your own personal data, and stored values are validated for type and size.
- Data is encrypted in transit (TLS) and at rest by Google Cloud.
- Attachments are verified with a SHA-256 fingerprint before a phone accepts them.

## Your choices

- **Leave a home** in Settings. Your shared history stays with that home, because other people's
  balances depend on it.
- **Delete your account** in Settings. This removes you from your home and permanently deletes
  your personal ledger, budgets, goals, accounts and sign-in.
- **Export** your personal ledger as CSV from the Personal screen.

## Contact

Questions or deletion requests: open an issue at
https://github.com/SE-Muhammad-Shamoil/fairsplit-releases/issues
