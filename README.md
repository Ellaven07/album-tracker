# Album Tracker

Album Tracker is a React web app for searching music albums, previewing their tracks, and keeping a personal listening log with statuses, ratings, and notes. It can play full albums through Deezer's embeddable player and suggest new albums with LLM-powered recommendations based on your saved albums and ratings.

**Screenshot:** _add a screenshot here_
**Live link:** (https://album-tracker-git-main-anica-ella.vercel.app/)

## Features

- Search albums and artists (iTunes Search API, no key needed)
- Album page with cover, year, genre, track list, and 30-second previews
- Links to listen on Spotify, YouTube, and Apple Music
- Mini player that keeps playing while you browse (play/pause, previous/next, seek)
- Personal collection with status, 1-5 star rating, notes, filter, and sort
- Optional full-album playback with Deezer's player
- LLM-powered recommendations based on the user's saved albums and ratings

## Tech stack

React, Vite, Context API, iTunes API, Deezer, Google Gemini, Vercel serverless functions

## Run locally

```bash
git clone https://github.com/YOUR-USERNAME/album-tracker.git
cd album-tracker
npm install
# create .env.local in the project root containing:
# GEMINI_API_KEY=your-key-here
npm run dev
```

## Limitations

- Previews are 30 seconds (all the iTunes API provides)
- The collection is saved only in your browser (localStorage)
- Deezer needs a login (and a plan that includes full tracks in your country) to play full tracks

## Privacy

The recommendations feature sends your saved albums' titles, artists, ratings, and statuses to Google's Gemini API. Your notes are not sent.

## Disclaimer

This is a learning project and is not affiliated with Apple, Spotify, Deezer, or Google. Music data, artwork, and audio belong to their owners.
