# NaviBeat Homebrew tap

The official [Homebrew](https://brew.sh) cask for [NaviBeat for Linux](https://navibeat.app/linux), a music player for Navidrome and other OpenSubsonic servers. It is meant for atomic distributions such as Fedora Atomic and Bazzite, where layering an RPM has a cost.

```sh
brew trust --tap nenadjokic/tap   # newer Homebrew asks for this once per third-party tap
brew install --cask nenadjokic/tap/navibeat-linux
```

It installs the full AppImage (with its own libVLC) for x86_64 and arm64, a `navibeat` command, and a launcher entry. `brew upgrade --cask navibeat-linux` moves to the latest release.

Linux only. NaviBeat for Mac is a separate app on the App Store.

The cask was written by [Jakob Hviid](https://github.com/jakobhviid/homebrew-tap), thank you.

Use this or the apt, dnf or pacman repository, not both: both install `navibeat` and a navibeat.desktop launcher.
