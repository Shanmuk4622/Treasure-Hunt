# Redesigned drop-in for the Treasure Hunt repo

These three files + `style.css` + the `assets/` folder are **drop-in replacements** for the original repo. The Supabase JS logic, table schemas, and RPC calls are unchanged — only markup classes/IDs the JS already targets are preserved, and the styling is replaced.

To use:
1. Replace `index.html`, `dashboard.html`, `admin.html`, `style.css` in your repo with these.
2. Copy `redesigned/assets/` → `assets/` at your repo root.
3. Plug in your `SUPABASE_URL` and `SUPABASE_ANON_KEY` (already filled in here from the source values).

What changed:
- **Doubloon-gold accent** for primary actions, focus states, score display, finished state
- **Cinzel display face** for the wordmark, "Treasure Hunt" hero, and "Congratulations!"
- **JetBrains Mono** for the secret-code field, leaderboard rank, and score
- **Compass-rose decoration** behind the auth card and in the header (~5–6% opacity)
- **Backdrop blur** on the modal overlay
- **Score pill** in the header (gold-tinted) instead of inline text
- **Improved leaderboard** — uppercase headers, hover row, monospace rank/score, gold rank-1, green "Finished!"
- All copy strings preserved verbatim from the source.
