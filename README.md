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
| [ČSFD](https://www.csfd.cz) | `csfd` | 1.1.0 | linux/x86_64, windows/x86_64 | ČSFD for movies and series: every title links to its page on csfd.cz (IDs from Wikidata), and ČSFD is a metadata source for titles that TMDB and IMDb do not know: search, found files and adding a title, with Czech plots, posters, ratings, cast and episodes. |
| File manager | `filemanager` | 1.5.0 | linux/x86_64, windows/x86_64 | Browse storage roots, preview files (text editor, images, media tracks and languages), create folders, rename, move and delete files (also many at once), upload files and folders. Changes only in roots marked as writable; moving a library file updates the title version. |
| [Histra.net](https://histra.net) | `histra` | 1.7.1 | linux/x86_64, windows/x86_64 | Track what you watch on histra.net: playback progress, watched titles, watchlist and lists in both directions. Also adds Histra IDs to your library. |
| [IMDb](https://www.imdb.com) | `imdb` | 1.1.0 | linux/x86_64, windows/x86_64 | IMDb as a metadata source for movies and series: search and match titles that TMDB does not know, with Czech, Slovak and English titles, ratings, seasons and episodes from the official IMDb datasets (non-commercial use). With a free OMDb API key it also adds plots, posters and age ratings. |
| [Jellyfin](https://jellyfin.org) | `jellyfin` | 1.2.4 | linux/x86_64, windows/x86_64 | One-way 1:1 copy of a Jellyfin server: movies and series exactly as Jellyfin has them (seasons, episode numbers, names, overviews, images, audio and subtitle tracks), and each user's watched titles, playback positions and favorites. |
| [Trakt](https://trakt.tv) | `trakt` | 1.2.0 | linux/x86_64, windows/x86_64 | Track what you watch on Trakt: scrobbling, watched titles, playback positions, watchlist, favorites and lists (direction per area), and Trakt IDs for your library. |
| [Webshare](https://webshare.cz) | `webshare` | 1.0.0 | linux/x86_64, windows/x86_64 | Add files from Webshare.cz to the library and play them with each viewer's own Webshare account. The direct link is created when playback starts and renewed when it expires. |
