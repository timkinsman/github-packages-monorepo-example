# @timkinsman/prettier-config

## Requirements

`"prettier": ">=3.0.0"`

## Installation

```sh
pnpm install -D @timkinsman/prettier-config
```

## Usage

```mjs
// .prettierrc.mjs

import timkinsmanPrettierConfig from "@timkinsman/prettier-config";

/**
 * @type {import("prettier").Config}
 */
const config = {
  ...timkinsmanPrettierConfig,
};

export default config;
```
