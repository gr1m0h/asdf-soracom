# asdf-soracom

[![Build](https://github.com/gr1m0h/asdf-soracom/actions/workflows/build.yaml/badge.svg)](https://github.com/gr1m0h/asdf-soracom/actions/workflows/build.yaml)
[![Lint](https://github.com/gr1m0h/asdf-soracom/actions/workflows/lint.yaml/badge.svg)](https://github.com/gr1m0h/asdf-soracom/actions/workflows/lint.yaml)

[soracom-cli](https://github.com/soracom/soracom-cli) plugin for the [asdf](https://github.com/asdf-vm/asdf) version manager.

## Install

```shell
asdf plugin add soracom https://github.com/gr1m0h/asdf-soracom.git
```

## Usage

See the [asdf documentation](https://asdf-vm.com/manage/core.html) for the full
set of commands. The most common ones are:

```shell
# Show all installable versions
asdf list all soracom

# Install a specific version
asdf install soracom latest
asdf install soracom 0.13.0

# Set a version globally (writes to ~/.tool-versions)
asdf set -u soracom latest

# Set a version for the current project (writes to ./.tool-versions)
asdf set soracom 0.13.0
```

## Contributing

Contributions are welcome! This plugin is linted with
[shellcheck](https://www.shellcheck.net/) and
[shfmt](https://github.com/mvdan/sh), and tested with
[asdf-vm/actions](https://github.com/asdf-vm/actions).

The required tooling versions are pinned in [`.tool-versions`](./.tool-versions),
so you can install them with asdf:

```shell
asdf install
```

```shell
# Format the shell scripts
./scripts/format.bash

# Lint the shell scripts
./scripts/lint.bash
```

## License

[MIT](./LICENSE)
