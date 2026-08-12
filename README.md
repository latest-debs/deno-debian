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

## Collaborate with us

latest-debs is a community effort — nobody "owns" this package and there's
no application to fill out. If you rely on it and want to help keep it
fresh, watching for a new upstream release or fixing a build hiccup, jump
in. Open an issue, send a PR, or drop into
[org discussions](https://github.com/orgs/latest-debs/discussions). Every
bit of help keeps this useful for everyone else who `apt install`s it.

## Disclaimer

Unofficial packaging only. For issues with deno itself, see
[denoland/deno](https://github.com/denoland/deno).
