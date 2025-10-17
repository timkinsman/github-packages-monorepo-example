# @timkinsman/eslint-config

## Requirements

`"eslint": ">=9.0.0"`

## Installation

```sh
pnpm install -D @timkinsman/eslint-config
```

## Usage

```cjs
// .eslint.config.mjs

import { FlatCompat } from "@eslint/eslintrc";
import js from "@eslint/js";
import { dirname } from "path";
import { fileURLToPath } from "url";

const __filename = fileURLToPath(import.meta.url);
const __dirname = dirname(__filename);

const compat = new FlatCompat({
  baseDirectory: __dirname,
  recommendedConfig: js.configs.recommended,
});

export default [
  // Apply your external config using FlatCompat
  ...compat.extends("@timkinsman/eslint-config"),
];

```
