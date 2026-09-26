![Spicy Player Banner](spicyplayer.png)

# Spicy Player (old)

> [!NOTE]
> **Looking for the Spicy Player lyrics app?** The new [Spicy Player](https://github.com/TheX24/spicy-player) shows Spicy Lyrics-style synced lyrics for whatever is playing in Spotify, YouTube Music or any other app. This repository is the earlier offline music player.

Spicy Player is an offline music player for Android with a port of [Spicy Lyrics](https://github.com/Spikerko/spicy-lyrics) - A [Spicetify](https://spicetify.app/) Extension, designed to achieve **visual parity** with Spicy Lyrics' rendering. Built using **Jetpack Compose (Canvas API)** and **ExoPlayer**.

> [!WARNING]
> This is a work in progress. The app is not yet complete and may have bugs.

## Project status: no longer developed

This offline music player has been succeeded by [Spicy Player](https://github.com/TheX24/spicy-player), a lyrics app that follows the music playing in other apps instead of managing its own library, queue, and playback. It carries on what this app was built for: the word-synced lyric renderer, the dynamic backgrounds and the synchronization work, plus many more lyrics sources and romanization. It installs as a separate app, so it won't replace or erase this one.

This repository stays up for reference, and its releases remain available, but it won't get new features or fixes.

---

## Key Features

- **Karaoke-style lyrics**: sub-pixel word/letter positioning, duet-aware left/right alignment, and a closed-form spring physics engine for scroll and word-bounce animation (frame-rate independent, no snap-back on seek).
- **Word-synced, line-synced, and static lyrics**, with RTL script support and on-device romanization (Japanese via Kuromoji, Chinese via pinyin4j).
- **Dynamic Background**: blurred cover-art backdrop, including a GPU shader-driven "Kawarp" engine alongside the legacy blur, selectable in settings.
- **Local library**: MediaStore-backed scanning of on-device music, with albums, playlists, and folder-based auto-pairing of audio files to their TTML lyrics.
- **Tag editor**: built-in metadata/tag editing (via jaudiotagger).

---

## Roadmap

Find the full feature and bug roadmap [here](https://lab.tx24.dev/b/9ihk5rxetqnK8awg6/project-spicy-player).

---

## Tech Stack

- **Jetpack Compose**: For the entire UI declaration and Canvas manipulation.
- **Media3 (ExoPlayer)**: Industrial-grade media decoding and playback.
- **Kotlin Coroutines**: For non-blocking IO during TTML and audio file scanning.
- **Custom XML Pull Parser**: For lightweight, low-memory performance on large lyric files.

## License

This project is licensed under the **AGPL-3.0 License**, inherited from the [Spicy Lyrics](https://github.com/Spikerko/spicy-lyrics) project. See the [LICENSE](LICENSE) file for the full text.

---

_Made by [TX24](https://tx24.is-a.dev) with the help of Antigravity and Claude Code. Based on [Spicy Lyrics](https://github.com/Spikerko/spicy-lyrics) - A [Spicetify](https://spicetify.app/) Extension_
