<sup>yoctocolors 🌈</sup>

> The smallest and fastest command-line coloring package on the internet. Trust me.

The only thing that matters is micro-benchmark performance! ⚡️

*Check out [Chalk](https://github.com/chalk/chalk) if you want something more mature and comprehensive.*

## Features

- **4x faster and 5x smaller than [nanocolors](https://github.com/ai/nanocolors)**
- Cat friendly
- An additional color
- Tree-shakeable but not stirred
- Actively maintained (at least for another week)
- No dependencies

## Install

```sh
npm install yoctocolors
```

## Usage

```js
import * as colors from 'yoctocolors';

console.log(colors.red('Yo!'));
```

## Styles

### Modifiers

- `reset` - Reset the current style.
- `bold` - Make the text bold.
- `dim` - Make the text have lower opacity.
- `italic` - Make the text italic. *(Not widely supported)*
- `underline` - Put a horizontal line above the text. *(Not widely supported)*
- `overline` - Put a horizontal line below the text. *(Not widely supported)*
- `inverse`- Invert background and foreground colors.
- `hidden` - Print the text but make it invisible.
- `strikethrough` - Put a horizontal line through the center of the text. *(Not widely supported)*

### Colors

- `black`
- `red`
- `green`
- `yellow`
- `blue`
- `magenta`
- `cyan`
- `white`
- `gray`

### Background colors

- `bgBlack`
- `bgRed`
- `bgGreen`
- `bgYellow`
- `bgBlue`
- `bgMagenta`
- `bgCyan`
- `bgWhite`
- `bgGray`

## Prior art

Yes

## Benchmark

```
❯ ./test/simple-benchmark.js
nanocolors    31508276 ops/sec
picocolors    32524769 ops/sec
yoctocolors   132894792 ops/sec
```

*Benchmark from [`nanocolors`](https://github.com/ai/nanocolors/blob/main/test/simple-benchmark.js)*
