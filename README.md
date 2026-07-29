## Hey — I'm 5w1tchy

Backend engineer working mostly in **Go**, with a side habit of building **Windows desktop tooling** — overlays, native input hooks, and self-updating apps.

Most of my day-to-day work lives in private team repos, so the list below is the honest version rather than the visible one.

---

### Tradewind — price-check overlay for Path of Exile 2

[`5w1tchy/tradewind-poe2`](https://github.com/5w1tchy/tradewind-poe2) · TypeScript, Electron, C++ · MIT

A hotkey overlay that reads the hovered in-game item and shows a price estimate at your cursor. I lead this one.

- **Native keyboard hook** (C++) so the hotkey fires while the game holds focus, driving a clipboard capture-and-restore loop — no memory reading, no injection, one game action per keypress.
- **Patch-resilient mod matching** — the stat database is pulled live from the trade API at startup and ETag-revalidated, so mods added in a new patch match on day one without shipping an app update.
- **Release pipeline** — GitHub Actions builds and publishes an NSIS installer on a version tag, with separate stable and pre-release update channels and background auto-update.
- Parser and stat matcher are covered by a test suite built from real in-game item copies.

Still early — the overlay, parser, and matcher work; live trade search and pricing are in progress.

---

### Production REST API *(private, team project)*

Go · PostgreSQL · Redis · S3-compatible object storage · Docker

Co-author on the backend of a multi-client content platform — one of two main contributors.

- Authentication, role and permission handling, subscription tiers, and an admin audit trail.
- Media upload and delivery through S3-compatible object storage, with Redis caching.
- Structured, typed error handling mapped cleanly from Postgres failures to API responses.
- Fully containerized development environment — API, database, cache, and storage all come up with a single Compose command.

---

### Smaller things

- **Wails desktop apps** in Go with web frontends
- **Go CLI utilities** — media clipping, scheduled data fetchers
- **Python** — Discord bots and a game project in progress
- **Laravel / TypeScript** — earlier full-stack work

---

### Stack

**Comfortable:** Go · TypeScript · Python · PostgreSQL · Docker · Redis
**Working knowledge:** Electron · Wails · C++ (native interop) · React · Vite

---

📫 Open to freelance and contract work — especially Go backends and Windows desktop tooling.
