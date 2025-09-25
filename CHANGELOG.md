# Changelog

All notable changes to this project will be documented in this file.  
The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## [Unreleased]

## [0.0.2] - 2025-09-25

### Added

- Syntax highlighting for `dup`, `eq`, and `neq` as `variable.language`.
- Syntax highlighting for `write` and `writeln` as `support.function`.
- Support for block comments `#[ ... ]#`.
- Customizable colors via `editor.tokenColorCustomizations`.

### Fixed

- Fixed conflict between line comments `#` and block comments `#[ ... ]#`.
- Updated scopes to use standard TextMate scopes (e.g. `keyword.control`, `constant.numeric`, `comment.line`) to ensure colors work across all themes.

## [0.0.1] - 2025-09-25

### Added

- Initial support for `.brz` files.
- Basic syntax highlighting for:
  - Keywords (`for`, `if`, `else`, `end`, etc.).
  - Numbers (decimal, hexadecimal, binary, octal, floating point).
  - Single and double quoted strings.
  - Line comments using `#`.
