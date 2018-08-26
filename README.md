# @ucudal/stylelint-config

This package provides UCUDAL's base CSS .stylelintrc as an extensible shared
config.

Extends
[`stylelint-config-standard`](https://github.com/stylelint/stylelint-config-standard).

## Usage

1. Install the correct versions of each peer dependency, which are listed by the
   command:

```sh
npm info "@ucudal/stylelint-config@latest" peerDependencies
```

Linux/OSX users can run:

```sh
(
  export PKG=@ucudal/stylelint-config;
  npm info "$PKG@latest" peerDependencies --json | command sed 's/[\{\},]//g ; s/: /@/g' | xargs npm install --save-dev "$PKG@latest"
)
```

Which produces and runs a command like:

```sh
npm install --save-dev @ucudal/stylelint-config@latest stylelint@^x.y.z
```

Windows users can install the `@ucudal/stylelint-config` and all its peer
dependencies manually.

2. Add `"extends": "@ucudal/stylelint-config"` to your `.stylelintrc` file.
