# VDF-Reader

## Introduction

VDF-Reader is a simple fork of [node-vdf](https://github.com/RJacksonm1/node-vdf) with a couple of modifications.

- VDF-Reader only offers a parser, no stringifier.
- VDF-Reader supports files with duplicate keys (like CS:GO's `items_game.txt`).

## Usage

```javascript
const vdf = require('vdf');

let string = fs.readFileSync('items_game.txt', 'utf8');
let parsed = vdf.parse(string);
```

## License

VDF-Reader is licensed under the MIT license.
