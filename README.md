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
toolkit --version
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

## Reporting issues

For bugs or feature requests related to the `toolkit` CLI itself, please open an issue on the [main repository](https://github.com/jingle2008/toolkit/issues).

For problems specific to installation via Homebrew, open an issue on [this tap repository](https://github.com/jingle2008/homebrew-toolkit/issues).

## License

Formula and cask files in this tap are generated automatically by [GoReleaser](https://goreleaser.com). The `toolkit` CLI is distributed under the license declared in its [upstream repository](https://github.com/jingle2008/toolkit).
