# homebrew-solitary

The Homebrew tap for [solitary](https://github.com/balakin/solitary) —
hypervisor-isolated cells for running coding agents off the leash.

```sh
brew install balakin/solitary/solitary
```

Homebrew resolves that name to this repository, installs
[Lima](https://lima-vm.io) alongside it — solitary drives `limactl` and has
nothing to run without it — and `brew upgrade solitary` keeps it current.

Casks install on macOS only. On Linux, use the install script:

```sh
curl -fsSL https://solitary.balakin.io/install.sh | sh
```

## This repository is generated

`Casks/solitary.rb` is written by GoReleaser from
[`.goreleaser.yaml`](https://github.com/balakin/solitary/blob/main/.goreleaser.yaml)
each time a release is published, and pushed here with a token that can write
nothing else. Editing the cask by hand only lasts until the next release —
change it in the main repository instead.
