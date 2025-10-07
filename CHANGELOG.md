# Changelog

All notable changes to this project will be documented in this file.  
The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## [Unreleased]

## [0.0.4] - 2025-10-07

### Added

- Added logical operators `and`, `or`, and `not` highlighted as `keyword.operator.logical`.
- Added `define` keyword to `keyword.control`.
- Added arithmetic operator highlighting for `**` (exponentiation) and `%` (modulo).
- Added comparison operators `<=` and `>=` to `keyword.operator.comparison`.
- Added general identifier highlighting rule (`variable.language`) to match valid names (`[a-zA-Z_][a-zA-Z0-9_+]*`).

### Changed

- Changed built-in stack and I/O words (`dup`, `eq`, `neq`, `write`, `writeln`, `over`, `swap`, `depth`, `dump`, `clear`, `rot`, `pop`) to use `keyword.other` for better visibility across themes.
- Split operator patterns into logical, comparison, and arithmetic groups for finer syntax coloring.
- Simplified numeric float matching pattern for better readability and consistency.
- Removed obsolete `constant.numeric.integer.int64` rule (unnecessary edge case).

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
