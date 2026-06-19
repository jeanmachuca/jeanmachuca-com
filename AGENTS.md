# jeanmachuca.com — Agent instructions

## Branching & PR flow

- **`main`** — production. Protected: requires PR with 1 review. Only merges from `development`.
- **`development`** — integration. Protected: requires PR with 1 review. Only merges from topic branches.
- **Topic branches** — create from `development`: `feature/<topic>`, `fix/<topic>`, `docs/<topic>`.
- PR flow: `feature|fix|docs/*` → PR → `development` → PR → `main`

### Exceptions

Direct pushes to `development` or `main` only when the user explicitly instructs it (e.g. emergency). Remind them this bypasses protection.

## No rebase

Use `git pull` (merge), never `git pull --rebase` or `git rebase`.

## Deploy

Push to `main` triggers GitHub Actions → GitHub Pages. No manual deploy needed.

## Images

- `images/headshot.jpg` — hero photo
- `images/nitroxr-game-center.jpg` — NitroXR project card
- `images/speaking/` — event photos for the Speaking gallery
