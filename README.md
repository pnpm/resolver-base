# @pnpm/resolver-base

> Types for pnpm-compatible resolvers

<!--@shields('npm', 'travis')-->
[![npm version](https://img.shields.io/npm/v/@pnpm/resolver-base.svg)](https://www.npmjs.com/package/@pnpm/resolver-base) [![Build Status](https://img.shields.io/travis/pnpm/resolver-base/master.svg)](https://travis-ci.org/pnpm/resolver-base)
<!--/@-->

## Installation

```sh
npm i -S @pnpm/resolver-base
```

## Usage

Here's a template of a resolver using types from `@pnpm/resolver-base`:

```ts
import {
  ResolveOptions,
  ResolveResult,
  WantedDependency,
} from '@pnpm/resolver-base'

export async function (
  wantedDependency: WantedDependency,
  opts: ResolveOptions,
): Promise<ResolveResult> {
  // ...
  return {
    id,
    resolution,
    package,
    latest,
    normalizedPref,
  }
}
```

## License

[MIT](./LICENSE) © [Zoltan Kochan](https://www.kochan.io/)
