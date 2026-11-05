# Kinovna plugins

Official plugin catalog for [Kinovna](https://github.com/michalss/kinovna). Packages are attached
to [releases](https://github.com/michalss/kinovna-plugins/releases), the catalog is [`index.json`](index.json).

## Use it in Kinovna

The catalog is preset on new servers. To add it, go to **Settings → Plugins → Plugin catalogs**:

```json
{ "Kinovna": "https://raw.githubusercontent.com/michalss/kinovna-plugins/main/index.json" }
```

Then install plugins in **Administration → Plugins → Catalog**. The scheduled task
**Update plugins** installs new versions automatically (can be switched off in Settings or per
plugin). A version that asks for new permissions is never installed automatically.

## Plugins

| Plugin | ID | Version | Platforms | Description |
|---|---|---|---|---|
| File manager | `filemanager` | 1.3.0 | linux/x86_64, windows/x86_64 | Browse storage roots, preview files (text editor, images, media tracks and languages), create folders, rename, move and delete files. Changes only in roots marked as writable; moving a library file updates the title version. |
| [Histra.net](https://histra.net) | `histra` | 1.5.0 | linux/x86_64, windows/x86_64 | Track what you watch on histra.net: playback progress, watched titles, watchlist and lists in both directions. |
| [Jellyfin](https://jellyfin.org) | `jellyfin` | 1.0.1 | linux/x86_64, windows/x86_64 | One-way sync from a Jellyfin server: movies and episodes from shared storage are added to the library, and each user's watched titles, playback positions and favorites follow. |
| [Trakt](https://trakt.tv) | `trakt` | 1.1.0 | linux/x86_64, windows/x86_64 | Track what you watch on Trakt: scrobbling, watched titles, playback positions, watchlist, favorites and lists (direction per area), and Trakt IDs for your library. |
