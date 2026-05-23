# Abrase syntax for Sublime Text

Syntax highlighting for the [Abrase](https://github.com/KHN190/Abrase) language (`.abe`).

## Install

### Package Control

Pending submission.

### Manual

```sh
git clone https://github.com/KHN190/Abrase-sublime \
  "$HOME/Library/Application Support/Sublime Text/Packages/Abrase"
```

(Adjust path for Linux / Windows. Restart Sublime Text.)

## Coverage

- `//` line comments
- string literals with `{ident}` interpolation, char literals
- decimal / hex integer and float literals
- all keywords including `handle`, `resume`, `region`, `effect`
- builtin types (`Int`, `Float`, `Bool`, `String`, `Unit`, `Char`)
- capitalized identifiers as types / variant constructors
- declaration name highlighting for `fn`, `type`, `effect`, `trait`

## License

MIT
