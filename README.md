# Beremiz VS Code Extension

Syntax highlighting support for the **Beremiz** language (`.brz` files) in Visual Studio Code.

This extension is intended for use with [Beremiz](https://github.com/AdaiasMagdiel/Beremiz-Go) (stack-based toy programming language implemented in Go).  
It provides syntax coloring, comment support, and basic editor features for `.brz` source files.

---

## Features

- 📄 **Syntax Highlighting**

  - Keywords (`for`, `if`, `do`, `elif`, `else`, `end`, etc.)
  - Built-in functions (`write`, `writeln`)
  - Stack operators (`dup`, `eq`, `neq`)
  - Constants (`true`, `false`, `nil`)
  - Numbers (decimal, binary, hex, octal, floats)
  - Strings (single and double quoted)
  - Comments (`# line`, `#[ block ]#`)

- 🎨 Works with all VS Code color themes
- ⚡ Lightweight TextMate grammar for fast parsing

---

## Example

```beremiz
10

for dup 0 neq do
 dup writeln
 1 -
end
```

---

## Changelog

See [CHANGELOG.md](./CHANGELOG.md) for release history.
