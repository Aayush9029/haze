<p align="center">
  <img src="assets/icon.png" width="128" alt="haze">
  <h1 align="center">haze</h1>
  <p align="center">Progressive blur, grain, and gradient color overlay for video</p>
</p>

<p align="center">
  <a href="https://github.com/Aayush9029/haze/releases/latest"><img src="https://img.shields.io/github/v/release/Aayush9029/haze" alt="Release"></a>
  <a href="https://github.com/Aayush9029/haze/blob/main/LICENSE"><img src="https://img.shields.io/github/license/Aayush9029/haze" alt="License"></a>
</p>

## Install

```bash
brew install aayush9029/tap/haze
```

Or tap first:

```bash
brew tap aayush9029/tap
brew install haze
```

Requires `ffmpeg` (`brew install ffmpeg`).

## Usage

```bash
haze in.mp4                                           # default progressive blur, ramped over the bottom 2/3
haze --no-noise --blur-max 30 in.mp4                  # softer blur, no grain
haze --overlay white in.mp4 out.mp4                   # add a white gradient fade on top
haze --overlay '#000000' --overlay-steepness 1.8 in.mp4
haze --bands 12 --preset ultrafast in.mp4             # fast preview
```

Run `haze --help` for the full list of options.

## License

MIT
