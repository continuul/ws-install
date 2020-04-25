[![license: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/continuul/ws-get/blob/master/LICENSE)

**Contents**

- [ws-get &mdash; introduction](#ws-get-mdash-introduction)
- [Examples](#examples)
- [Installing ws](#installing-ws)
  - [Manual installation](#manual-installation)
- [Updating ws](#updating-ws)
  - [Manual updating](#manual-updating)
- [Uninstalling ws](#uninstalling-ws)
  - [Manual uninstallation](#manual-uninstallation)
- [License](#license)

# ws-get &mdash; introduction

**Installs [`ws`][ws]**, the **Developer Workspace Manager**, on Unix-like platforms.
Additionally, install script subcommands `ws-get update` for later on-demand updating of `ws`, and `ws-get uninstall` for uninstalling.

The simplest case is **installation of `ws` with confirmation prompt**:

```shell
curl -L https://git.io/ws-get | bash
```

## Examples

See [Installation options](#installation-options) for details.

* Installation with confirmation prompt to default location `$HOME/ws`:

```shell
curl -L https://git.io/ws-get | bash
```

* Automated installation to default location `$HOME/ws` with no confirmation prompt:

```shell
curl -L https://git.io/ws-get | bash -s -- -y
```

* Automated, _quiet_ installation to default location `$HOME/ws`; _no status information_
is displayed:

```shell
curl -sL https://git.io/ws-get | bash -s -- -q
```

## Installation from GitHub

```shell
curl -L https://git.io/ws-get | [WS_PREFIX=<dir>] bash [-s -- [-y] [<subcommand>...]]
```

## Updating ws

Run `ws-get update` on demand to update `ws` itself to the latest version.

`ws-get update -y` skips the confirmation prompt.

## Uninstalling ws

Run `ws-get uninstall` to uninstall `ws` without deleting any workspaces.

`ws-get uninstall -y` skips the confirmation prompt - **use with caution**.

## License

Copyright (c) 2016-2020 continuul.io, released under the [MIT license](https://spdx.org/licenses/MIT#licenseText).

  [ws]: https://github.com/continuul/ws
