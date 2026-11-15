# Albumdle Issue Tracker

Public bug tracker and data-troubleshooting guide for Albumdle.

- **[Play Albumdle](https://albumdle.wtf)**
- **[Open a New Issue](https://github.com/LeonMontealegre/Albumdle-issues/issues/new/choose)**

---

## Before Reporting a Missing or Incorrect Album

Albumdle builds its catalog from open community music databases rather than a private curated list:

- **[MusicBrainz](https://musicbrainz.org/)**: Community-edited music encyclopedia (like Wikipedia for music metadata) providing albums, release dates, tracklists, runtimes, labels, genres, contributors, and **[Cover Art Archive](https://musicbrainz.org/doc/Cover_Art_Archive)** images.
- **[ListenBrainz](https://listenbrainz.org/)**: Open listening-history companion used for artist and album play-count thresholds.
- **[Last.fm](https://www.last.fm/)**: Used for **Artist Popularity** listener tiers.
- **[theneedledrop](https://theneedledrop.com/) / Stas Deep**: Used for optional **Fantano Scores** (matched by album & artist title).

Because anyone can edit MusicBrainz, fixing missing or wrong album metadata there is the best way to get it fixed in Albumdle (changes appear after Albumdle's next periodic dataset snapshot), and helps the music community as a whole :)!

### Requirements for an Album to Appear in Albumdle

**Artist Requirements (MusicBrainz + ListenBrainz):**
- Artist type is **Group** or **Person**
- Has a **Wikipedia or Wikidata** external link
- Has a **Spotify, Apple Music, or Bandcamp** URL
- Not primarily tagged `classical` or `conductor` (unless outvoted by another genre tag)
- Has **> 12,500 total plays** in ListenBrainz

**Album (Release Group) Requirements (MusicBrainz + ListenBrainz):**
- Primary type is **Album** *(EPs and Singles are excluded)*
- Secondary type is studio (none), **Mixtape/Street**, **Live**, or **Soundtrack** *(Compilations, Remixes, DJ-mixes, Spokenword, etc. are excluded)*
- Has at least one **Official** release with **> 0 tracks**
- Has cover art uploaded to the **Cover Art Archive**
- Has at least one recognized **MusicBrainz genre tag** (`count >= 0`, checked on the Release Group first, then Artist, then the Artist's other Release Groups)
- Meets **ListenBrainz** play thresholds (`> 500` album plays & meaningful artist share, or released within ~6 months)

---

## What Belongs in This Tracker?

Please open an issue here for:
- **Website / UI / gameplay bugs** (layout glitches, search/filter issues, local state bugs, etc.)
- **Albumdle-side data mismatches** that you already verified on MusicBrainz / Last.fm (for example, a mismatched Fantano score or data that meets all rules above)
- **Feature requests & feedback**

For routine metadata fixes, please check or update **[MusicBrainz](https://musicbrainz.org/doc/How_to_Contribute)** first!
