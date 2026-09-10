# homebrew-tap

Homebrew formulae by [@tomekceszke](https://github.com/tomekceszke).

## tubeamp

[TubeAmp](https://github.com/tomekceszke/tubeamp) — a retro-styled terminal music
player that streams audio from YouTube.

```bash
brew install tomekceszke/tap/tubeamp
tubeamp
```

The formula declares mpv and ffmpeg, so the two libraries TubeAmp loads through
ctypes and shells out to come along with it. Nothing else to install.

Installing by the full name trusts this one formula, which is all Homebrew needs.
Trusting the whole tap is broader and unnecessary.

### Playback stopped working?

YouTube changes often enough that a pinned yt-dlp goes stale, and this formula
pins one. That is what a broken video usually means:

```bash
brew upgrade tubeamp
```

Linux, WSL2, and installing from PyPI with `uv` or `pipx` are covered in the
[main repository](https://github.com/tomekceszke/tubeamp).
