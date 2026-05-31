# 🎬 CineFlow

A personal movie and TV streaming tracker built as a single HTML file. Discover, track, and watch movies and series with a clean Netflix-inspired interface.

---

## ✨ Features

- **Browse & Discover** — Trending, Top Rated, Top 10 Today, and genre filtering for both movies and series
- **Watch Movies & Series** — Powered by NexStream embed API
- **YouTube Trailers** — Auto-fetched for every title using TMDB
- **Episode Guide** — Full season/episode browser with descriptions, thumbnails, runtime, and watched indicators
- **Continue Watching** — Remembers exactly which episode and season you were on
- **Skip Intro & Next Episode** — Skip intro button at the start of episodes, auto next episode countdown before the end
- **User Accounts** — Register and sign in with local accounts (stored in browser)
- **Watchlist** — Save movies and series to watch later
- **Watch History** — Tracks everything you've watched with dates
- **Trakt.tv Sync** — Connect your Trakt account to sync watch history and watchlist bidirectionally
- **Cast & Crew** — Full cast with photos and character names
- **More Like This** — Similar titles shown on every movie and series page
- **IMDb Ratings** — Shown on every title
- **Profile Editing** — Change username, password, and profile photo
- **Search** — Live search powered by TMDB
- **Horizontal Scrolling Rows** — Netflix-style rows with arrow navigation

---

## 🛠️ Built With

- Plain HTML, CSS, JavaScript — no frameworks, no build tools
- [TMDB API](https://www.themoviedb.org/documentation/api) — movie and series data, posters, trailers, cast
- [NexStream API](https://api.codespecters.com) — movie and series streaming embeds
- [Trakt.tv API](https://trakt.tv/b/api-docs) — watch history and watchlist sync
- [YouTube](https://youtube.com) — trailer embeds via youtube-nocookie

---

## 🚀 Setup

### 1. Get API Keys

| Service | Where to get it | Free |
|---|---|---|
| TMDB | [themoviedb.org/settings/api](https://www.themoviedb.org/settings/api) | ✅ |
| NexStream | [api.codespecters.com](https://api.codespecters.com) | ✅ |
| Trakt | [trakt.tv/oauth/applications/new](https://trakt.tv/oauth/applications/new) | ✅ |

### 2. Add Your Keys

Open `index.html` and find these lines near the top of the `<script>` tag:

```js
const TMDB_KEY = 'your_tmdb_key';
const TRAKT_CLIENT_ID = 'your_trakt_client_id';
const NEXSTREAM_KEY = 'your_nexstream_key';
const TRAKT_PIN_URL = `https://trakt.tv/pin/your_app_pin_id`;
```

Replace each value with your own keys.

### 3. Run It

Just open `index.html` in any browser. No server or install needed.

---

## 🔗 Trakt Setup

1. Go to [trakt.tv/oauth/applications/new](https://trakt.tv/oauth/applications/new)
2. Set **Redirect URI** to `urn:ietf:wg:oauth:2.0:oob`
3. Save and copy your **Client ID** and **App PIN ID** from the URL
4. In the app go to **History tab** → **Connect Trakt**
5. Approve on Trakt, paste the PIN back → done

---

## 📁 Project Structure

```
index.html   ← entire app in one file
README.md    ← this file
```

---

## ⚠️ Disclaimer

This project uses third-party streaming embeds. It is intended for personal and educational use only. The developer does not host or distribute any copyrighted content.

---

## 🙋 Author

Built by **Obaid** — pre-engineering student from Karachi, Pakistan.

> Made with curiosity, late nights, and a lot of debugging.
