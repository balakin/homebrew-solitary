# homebrew-solitary

The Homebrew tap for [solitary](https://github.com/balakin/solitary) —
hypervisor-isolated cells for running coding agents off the leash.

```sh
brew install balakin/solitary/solitary
```

Homebrew resolves that name to this repository, installs
[Lima](https://lima-vm.io) alongside it — solitary drives `limactl` and has
nothing to run without it — and `brew upgrade solitary` keeps it current. This
is a formula rather than a cask, so it works on Linux as well as macOS.

Without Homebrew, the install script does the same job on both:

```sh
curl -fsSL https://solitary.balakin.io/install.sh | sh
```

## This repository is generated

`Formula/solitary.rb` is written by GoReleaser from
[`.goreleaser.yaml`](https://github.com/balakin/solitary/blob/main/.goreleaser.yaml)
each time a release is published, and pushed here with a token that can write
nothing else. Editing the formula by hand only lasts until the next release —
change it in the main repository instead.
