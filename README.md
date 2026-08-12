![deno for Debian](.github/readme-header.png)

# deno for Debian

[deno](https://github.com/denoland/deno) — a modern runtime for JavaScript
and TypeScript — packaged for Debian as part of
[latest-debs](https://github.com/latest-debs).

## Install

Via the latest-debs apt repository:

```sh
sudo extrepo enable latest-debs
sudo apt update
sudo apt install deno
```

Or download a `.deb` from the [Releases](https://github.com/latest-debs/deno-debian/releases) page:

```sh
sudo dpkg -i deno_*.deb
```

## Supported distributions & architectures

- Debian Bookworm (12), Trixie (13), Forky (14/testing), Sid (unstable)
- amd64, arm64

  (deno's upstream releases only publish amd64/arm64 Linux binaries)

## Building

Run the [Build deno for Debian](../../actions) workflow on GitHub with the
desired upstream version. Packaging is driven by
[debian-multiarch-builder](https://github.com/ranjithrajv/debian-multiarch-builder).

## Disclaimer

Unofficial packaging only. For issues with deno itself, see
[denoland/deno](https://github.com/denoland/deno).
