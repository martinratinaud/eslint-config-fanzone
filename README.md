# FanZone ESLint config

ESLint config for FanZone JavaScript code.

## Table of Contents

1. [Overview](#overview)
2. [License](#license)
3. [Dependencies](#dependencies)
4. [Usage](#usage)

## Overview

In order to standardize and enforce FanZone's JavaScript coding style across multiple codebases, FanZone has adopted ESLint and this shared ESLint config. This document describes the FanZone JavaScript style and its inspirations.

## License

The code in this repository is released under the Apache 2.0 license unless otherwise
noted. Please see the [LICENSE file](https://github.com/fanzone/eslint-config-fanzone/blob/master/LICENSE) for details.

## Dependencies

[ESLint](http://eslint.org) is required to use `eslint-config-fanzone`, as it is an [ESLint shareable config](http://eslint.org/docs/developer-guide/shareable-configs).

## Usage

As this package is held on a private repo, you may want to install it through link, so in this folder, run

    npm link
    # or
    yarn link

To begin using the FanZone ESLint config in a codebase, first install ESLint and the config:

    yarn add --dev eslint
    yarn link eslint-config-fanzone

Then, configure your project's ESLint config to extend `eslint-config-fanzone` (see the ESLint docs on [Using a Shareable Config](http://eslint.org/docs/developer-guide/shareable-configs#using-a-shareable-config))

Basically, create a `.eslintrc` file with this inside

```json
{
  "extends": "fanzone"
}
```
