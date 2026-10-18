# Contributing to Larus

Larus is a flight instrument maintained with limited time. Correctness
matters more than speed, and review time is limited. So: discuss first,
code second.

## How to contribute

1. **Open an issue** describing the problem and your proposed approach.
   For bugs, include version, hardware setup, and steps to reproduce
   (a log file helps).
2. **Wait for the `accepted` label.** Only maintainers set it.
3. **Open a pull request** that links the issue (`Closes #123`).

Pull requests without an accepted issue may be closed without review.
**Exception:** typo fixes and small documentation corrections.

## Interface changes: specification first

Changes to the CAN spec, NMEA protocol, LRSX log format, or EEPROM layout
must first be merged as a specification change in
[`doc_larus`](https://github.com/larus-breeze/doc_larus). Only then submit
the implementation, referencing that change. This also applies to
"small" documentation fixes in these specifications.

## Pull requests

- One topic per pull request. No unrelated refactoring, renaming,
  reformatting, or dependency upgrades.
- Everything in English.
- Describe what changed, why, and **how you tested it** (hardware or the
  SIL simulator in [`sw_tools`](https://github.com/larus-breeze/sw_tools)).
  Untested changes to flight-relevant code are not merged.
- Algorithm changes go to
  [`sw_algorithms_lib`](https://github.com/larus-breeze/sw_algorithms_lib)
  first; submodule references must point to its `main` branch.

## AI-assisted contributions

Welcome, under the same rules, plus:

- State which AI tool you used and how.
- You must understand every line and answer review questions yourself.
- If you use a coding agent, make sure it reads the repository's
  `AGENTS.md`.

## License

Contributions are licensed under the repository's license: GPL-3.0 for
software, CC BY-SA 4.0 for `doc_larus`.
