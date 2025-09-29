# Changelog

All notable changes to this project will be documented in this file.  
The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## [Unreleased]

## [0.0.3] - 2025-09-29

### Added

- Added `type` to `keyword.control`.
- Added stack/utility words (`over`, `swap`, `depth`, `dump`, `clear`, `rot`, `pop`) to `variable.language`.

### Changed

- Expanded `variable.language` group to include all stack manipulation and I/O words for consistent highlighting.

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
