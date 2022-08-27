# @esm2cjs/ip-regex

This is a fork of https://github.com/sindresorhus/ip-regex, but automatically patched to support ESM **and** CommonJS, unlike the original repository.

## Install

You can use an npm alias to install this package under the original name:

```
npm i ip-regex@npm:@esm2cjs/ip-regex
```

```jsonc
// package.json
"dependencies": {
    "ip-regex": "npm:@esm2cjs/ip-regex"
}
```

but `npm` might dedupe this incorrectly when other packages depend on the replaced package. If you can, prefer using the scoped package directly:

```
npm i @esm2cjs/ip-regex
```

```jsonc
// package.json
"dependencies": {
    "@esm2cjs/ip-regex": "^ver.si.on"
}
```

## Usage

```js
// Using ESM import syntax
import ipRegex from "@esm2cjs/ip-regex";

// Using CommonJS require()
const ipRegex = require("@esm2cjs/ip-regex").default;
```

> **Note:**
> Because the original module uses `export default`, you need to append `.default` to the `require()` call.

For more details, please see the original [repository](https://github.com/sindresorhus/ip-regex).

## Sponsoring

To support my efforts in maintaining the ESM/CommonJS hybrid, please sponsor [here](https://github.com/sponsors/AlCalzone).

To support the original author of the module, please sponsor [here](https://github.com/sindresorhus/ip-regex).
