# Morning Brief

A minimal daily dashboard designed to live on your iPhone home screen. Every morning it shows you the five things that matter most that day — with direct links to emails, docs, or anything else you need to act on them.

## Features

- **Five priorities** — set them the night before, wake up to a clean focused view
- **Linked resources** — attach Gmail links, Google Docs, calendar events, or any URL to each priority so you can jump straight into the work
- **Tap to complete** — mark items done throughout the day with a gold progress bar tracking your streak
- **Daily quote** — a rotating motivational note at the bottom
- **Resets daily** — done states clear automatically each morning so you always start fresh
- **Works offline** — no server, no account, no tracking; your data stays on your device

## Install on iPhone

1. Deploy to Vercel (see below)
2. Open your Vercel URL in **Safari** on your iPhone
3. Tap the **Share** button → **Add to Home Screen**
4. Name it "Morning Brief" and tap Add

It will appear on your home screen and open full-screen, no browser chrome.

## Automate the Morning Pop-Up

Use the iOS Shortcuts app to have it open automatically each morning:

1. Open **Shortcuts** → **Automation** → tap **+**
2. Choose **Time of Day** → set your wake-up time → **Run Immediately**
3. Add action: **Open URLs** → paste your Vercel URL
4. Save

## Deploy to Vercel

**What you need:** A GitHub account and a Vercel account (both free).

1. Create a new GitHub repository named `morning-brief`
2. Add both files to the root of the repo:
   - `index.html`
   - `vercel.json`
3. Go to [vercel.com](https://vercel.com) → **Add New Project**
4. Import your `morning-brief` GitHub repo
5. Click **Deploy** — your site will be live in ~30 seconds

Vercel will give you a URL like `morning-brief.vercel.app`. You can customize this in your Vercel project settings.

Any time you push an update to GitHub, Vercel redeploys automatically.

## How to Use

**Evening (set your list):**
1. Open the app → tap **Edit tomorrow's list**
2. Type your five priorities in order of importance
3. For each one, tap **Add link** to attach relevant URLs (Gmail messages, Docs, calendar events, etc.)
4. Tap **Save & Set**

**Morning (work your list):**
1. App opens to your priorities for the day
2. Tap any gold link chip to open the associated email or document directly
3. Tap the priority text area to mark it done — a checkmark appears and the progress bar advances

## Data & Privacy

All data is stored in your browser's local storage — it never leaves your device and is not sent to any server. Clearing Safari's website data will erase your saved priorities.

## Files

```
morning-brief/
├── index.html      # The entire app (single file, zero dependencies)
├── vercel.json     # Vercel routing config
└── README.md       # This file
```

## Future Ideas

- Cloud sync so priorities persist across devices
- AI-assisted priority drafting from Gmail/Calendar
- Streak tracking and weekly review view
- Widget support via iOS Shortcuts
