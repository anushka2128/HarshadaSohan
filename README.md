# Harshada & Sohan – Wedding Invitation

Interactive digital wedding invitation for **Harshada Shinde & Sohan Chougule**.

## Project Structure
- `public/index.html` – The complete interactive invitation (envelope zipper opening, automatic Page 2 preview illusion, scratch-and-reveal lagna muhurat, countdown, event schedule, Google Maps & calendar integration, realtime blessings wall, and Excel export).
- `public/firebase-config.js` – Firebase Firestore configuration for realtime live blessings and anonymous authentication.
- `public/img/` – Maharashtrian wedding artwork (bells, couple arch, muhurat lamps, sohola arch, watercolor florals).
- `public/Sajiri-Gojiri.mp3` – Background wedding music with audio controls and Web Audio synthesiser fallback.
- `firestore.rules` – Firestore security rules allowing public reads, anonymous posts, and author-only deletions.
- `netlify.toml` – Netlify deployment configuration (`publish = "public"`).

## Deployment

### Option A – Netlify (Recommended)
1. Push this repository to GitHub.
2. In Netlify, select **Add new site** > **Import an existing project** > choose your repository.
3. The publish directory is set to `public` in `netlify.toml`.
4. Deploy the site and share the link.

### Option B – Firebase Hosting
```bash
npm install -g firebase-tools
firebase login
firebase init hosting
firebase deploy
```

## Features
- **Royal Envelope Opening**: Interactive gold seal and zipper slide-to-open gesture with twinkling dust and flower petal shower.
- **Automatic Preview Peek**: After the envelope opens and Page 1 entrance finishes, the invitation automatically and smoothly scrolls to peek at Page 2, naturally showing guests to scroll down.
- **Scratch Card Shubh Muhurat**: Interactive touch/mouse scratch card revealing wedding date and time, with swipeable panels and automated demo.
- **Realtime Blessings & Ukhane Wall**: Powered by Firebase Firestore with offline fallback; guests can post blessings or rhyming ukhane, delete their own posts, and export all messages to a formatted Excel (.xlsx) spreadsheet.
- **Responsive Layout**: Designed for all mobile devices, tablets, and desktop displays with authentic Paithani border styling.
