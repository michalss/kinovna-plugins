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
| Autopilot | `autopilot` | 1.10.0 | linux/x86_64, windows/x86_64 | Automatic TV series downloads (replaces Sonarr): follows series on TMDB, finds missing episodes through the Search plugin and other sources, picks the best release by quality profile (resolution, Czech dubbing and subtitles, size), downloads it with Torrent, Usenet or file hosts and moves finished episodes into the series folder. Imports series and profiles from Sonarr. |
| Bugs & requests | `bugs` | 1.3.2 | linux/x86_64, windows/x86_64 | Tracker for Kinovna itself: bugs, new features and change requests with priority, version and the platforms they affect (server, web, desktop, Android, Android TV, iOS, tvOS, Tizen, webOS), votes and a conversation with mentions and images. Developers take items and track their status separately on each platform, including the version with the fix. |
| [ČSFD](https://www.csfd.cz) | `csfd` | 1.1.1 | linux/x86_64, windows/x86_64 | ČSFD for movies and series: every title links to its page on csfd.cz (IDs from Wikidata), and ČSFD is a metadata source for titles that TMDB and IMDb do not know: search, found files and adding a title, with Czech plots, posters, ratings, cast and episodes. |
| [FastShare](https://fastshare.cz) | `fastshare` | 1.0.0 | linux/x86_64, windows/x86_64 | Search FastShare.cz and download files into the storage with your FastShare account. Works through the plugin bus: results and downloads appear in the Search plugin. |
| File manager | `filemanager` | 1.10.0 | linux/x86_64, windows/x86_64 | Browse storage roots, preview files (text editor, images, media tracks and languages), create folders, rename, move, copy and delete files (also many at once), upload files and folders, rename video files to release-style names from metadata (library title, or the file name outside the library). Changes only in roots marked as writable; moving a library file updates the title version. |
| [Histra.net](https://histra.net) | `histra` | 1.8.7 | linux/x86_64, windows/x86_64 | Track what you watch on histra.net: playback progress, watched titles, watchlist and lists in both directions. Also adds Histra IDs to your library. |
| [IMDb](https://www.imdb.com) | `imdb` | 1.1.0 | linux/x86_64, windows/x86_64 | IMDb as a metadata source for movies and series: search and match titles that TMDB does not know, with Czech, Slovak and English titles, ratings, seasons and episodes from the official IMDb datasets (non-commercial use). With a free OMDb API key it also adds plots, posters and age ratings. |
| [Jellyfin](https://jellyfin.org) | `jellyfin` | 1.2.5 | linux/x86_64, windows/x86_64 | One-way 1:1 copy of a Jellyfin server: movies and series exactly as Jellyfin has them (seasons, episode numbers, names, overviews, images, audio and subtitle tracks), and each user's watched titles, playback positions and favorites. |
| [Media editor](https://mkvtoolnix.download) | `mediaedit` | 1.1.0 | linux/x86_64, windows/x86_64 | Edit tracks of MKV files: rename tracks, change languages and default/forced flags (instantly, without rewriting the file), add subtitles and audio, remove and reorder tracks, extract subtitles; other plugins (Autopilot) can have subtitles in unwanted languages removed through the plugin bus. Uses MKVToolNix, which the plugin can download and install by itself. |
| [MediaFlux](https://webshare.cz) | `mediaflux` | 1.3.0 | linux/x86_64, windows/x86_64 | Search the MediaFlux catalogue (movies and TV episodes with titles, year, quality and languages) and download the files from Webshare into the storage with a Webshare token. The encrypted file header is decrypted after the download. Works through the plugin bus: results and downloads appear in the Search plugin. |
| Reports | `reports` | 1.1.0 | linux/x86_64, windows/x86_64 | Users report problems with movies, series and episodes in the library (picture, sound, subtitles, playback, stream, metadata) right from the title page, together with the file (version) and playback position they were streaming; others can confirm them and discuss them in comments. Operators take reports, then close them as resolved or dismissed. |
| Requests | `requests` | 1.1.0 | linux/x86_64, windows/x86_64 | Users request movies and series that are not in the library (searched on TMDB), join others' requests and discuss them in comments. Operators take requests, then close them as done or rejected. |
| [Search](https://github.com/michalss/kinovna-plugins) | `search` | 1.5.0 | linux/x86_64, windows/x86_64 | Search trackers (Prowlarr definitions, no Prowlarr needed), newznab and torznab indexers and other plugins in one place and send a result to the Torrent or Usenet plugin. |
| [Titulky.com](https://www.titulky.com) | `titulky` | 1.0.1 | linux/x86_64, windows/x86_64 | Czech and Slovak subtitles from titulky.com: offered in the subtitle search of each title version (episodes matched exactly by the series, release matches first) and on the Titulky.com page with the latest subtitles, search, translations in progress and saving next to videos. |
| [Torrent](https://github.com/ikatson/rqbit) | `torrent` | 1.2.0 | linux/x86_64, windows/x86_64 | Torrent client: add magnet links or .torrent files, pick the files and the storage folder, watch progress, speed and peers, pause, resume and remove downloads; seeding stops at the configured ratio and the user is notified when a download finishes. Other plugins can add and control torrents through its local API. |
| [Trakt](https://trakt.tv) | `trakt` | 1.2.1 | linux/x86_64, windows/x86_64 | Track what you watch on Trakt: scrobbling, watched titles, playback positions, watchlist, favorites and lists (direction per area), and Trakt IDs for your library. |
| [Usenet](https://github.com/TheDancingDeveloper-org/rustnzb) | `usenet` | 1.1.1 | linux/x86_64, windows/x86_64 | Usenet (NZB) downloader: several providers with their own connection counts and priorities, PAR2 repair and unpacking, downloads straight into storage folders with progress, speed, pause, resume and history; the user is notified when a download finishes. Other plugins can add and control downloads through its local API. |
| [Webshare](https://webshare.cz) | `webshare` | 1.1.1 | linux/x86_64, windows/x86_64 | Add files from Webshare.cz to the library and play them with each viewer's own Webshare account. The direct link is created when playback starts and renewed when it expires. Other plugins (Search) can search Webshare and download files into the storage. |
