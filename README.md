# Abrase for Sublime Text

Syntax highlighting and a build system for the
[Abrase](https://github.com/KHN190/Abrase) language (`.abe`).

## Install

### Package Control

In Sublime Text, `cmd + P`, search for `Abrase`.

### Manual

```sh
git clone https://github.com/KHN190/Abrase-sublime \
  "$HOME/Library/Application Support/Sublime Text/Packages/Abrase"
```

(Adjust path for Linux / Windows. Restart Sublime Text.)

## Build system

`Tools → Build System → Abrase`, then:

- **Build** (`cmd+B`) — `abrase check`; errors are clickable (parsed from the
  `at line N, col N` output).
- **Build With…** (`cmd+shift+B`) — `Run`, `Run (debug)` (`--debug`), `Disasm`,
  `Explain`.

Needs the `abrase` CLI on `PATH`.

## Coverage

- `//` line and `/* */` block comments
- string literals with `{expr}` interpolation, char literals, escape sequences
- decimal / hex / binary integer and float literals
- all keywords: `handle`, `resume`, `throw`, `region`, `exn`, `return`, `use`, `static`, `op`, `alias`, `effect`, …
- attributes: `@derive`, `@export`, `@copy`, `@move`, `@share`, …
- builtin types (`Int`, `Float`, `Bool`, `String`, `Unit`, `Char`)
- capitalized identifiers as types / variant constructors
- declaration name highlighting for `fn`, `type`, `effect`, `trait`
- operators: arithmetic, comparison, logical, bitwise (`^`, `<<`, `>>`), range (`..`, `..=`), `::` path separator

## License

MIT
