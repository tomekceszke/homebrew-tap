# homebrew-tubeamp

Homebrew formula for [TubeAmp](https://github.com/tomekceszke/tubeamp) — a
retro-styled terminal music player that streams audio from YouTube.

```bash
brew install tomekceszke/tubeamp/tubeamp
tubeamp
```

The formula declares mpv and ffmpeg, so the two system libraries TubeAmp needs
come along with it. Nothing else to install.

## Playback stopped working?

YouTube changes often enough that a pinned yt-dlp goes stale, and this formula
pins one. That is what a broken video usually means:

```bash
brew upgrade tubeamp
```

## Other ways in

The [main repository](https://github.com/tomekceszke/tubeamp) covers Linux, WSL2
and installing from PyPI with `uv` or `pipx`.
