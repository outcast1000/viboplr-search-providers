# Viboplr — Web Search

Adds a Search submenu to artists, albums, and tracks for looking them up on Google, Last.fm, X, YouTube, Genius, and your own custom providers.

Externalized from [Viboplr](https://viboplr.com)'s built-in plugins — same code, now shipped as a standalone gallery plugin (id `search-providers`).

## Layout
- `manifest.json` — plugin metadata and contributions.
- `index.js` — the plugin code (ES5, executed via `new Function("api", code)`).
- `scripts/` — `bump.sh` (version + changelog) and `package.sh` (build `search-providers.zip` + `update.json`).

## Releasing
See [RELEASING.md](./RELEASING.md): `scripts/bump.sh <patch|minor|major>`, fill the changelog, commit, then push a `vX.Y.Z` tag — CI builds `search-providers.zip` + `update.json` and publishes the release.
