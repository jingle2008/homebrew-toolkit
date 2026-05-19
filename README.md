# homebrew-toolkit

Official [Homebrew](https://brew.sh) tap for [`toolkit`](https://github.com/jingle2008/toolkit) — a cross-platform command-line tool for cloud and infrastructure automation.

## Install

```sh
brew install jingle2008/toolkit/toolkit
```

This adds the tap and installs the latest release in one step. To tap explicitly first:

```sh
brew tap jingle2008/toolkit
brew install toolkit
```

### Cask (pre-built binary)

A cask is also available if you prefer the pre-built distribution:

```sh
brew install --cask jingle2008/toolkit/toolkit
```

## Supported platforms

| OS    | Architecture       |
| ----- | ------------------ |
| macOS | Intel (`amd64`)    |
| macOS | Apple Silicon (`arm64`) |
| Linux | Intel (`amd64`)    |
| Linux | ARM (`arm64`)      |

## Verify your install

```sh
toolkit version
```

## Upgrade

```sh
brew update
brew upgrade toolkit
```

## Uninstall

```sh
brew uninstall toolkit
brew untap jingle2008/toolkit
```

## Troubleshooting

### macOS: "toolkit cannot be opened" / "developer cannot be verified"

The macOS Gatekeeper blocks binaries downloaded from the internet that are not code-signed and notarized by Apple. The released `toolkit` binary is not yet notarized, so macOS quarantines it on first run.

Remove the quarantine attribute after install:

```sh
xattr -dr com.apple.quarantine "$(brew --prefix)/bin/toolkit"
```

If you installed via the cask, you can also bypass quarantine at install time:

```sh
brew install --cask --no-quarantine jingle2008/toolkit/toolkit
```

Either approach is safe for a binary you trust. Notarization is being tracked upstream in [jingle2008/toolkit](https://github.com/jingle2008/toolkit/issues).

## Reporting issues

For bugs or feature requests related to the `toolkit` CLI itself, please open an issue on the [main repository](https://github.com/jingle2008/toolkit/issues).

For problems specific to installation via Homebrew, open an issue on [this tap repository](https://github.com/jingle2008/homebrew-toolkit/issues).

## License

Formula and cask files in this tap are generated automatically by [GoReleaser](https://goreleaser.com). The `toolkit` CLI is distributed under the license declared in its [upstream repository](https://github.com/jingle2008/toolkit).
