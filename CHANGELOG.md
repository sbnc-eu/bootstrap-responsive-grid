# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.1.5] - 2021-04-26
### Changed
- Improved the clarity of explanations in the Readme.

## [1.1.4] - 2020-09-21
### Fixed
- Removed forgotten debug statement.

## [1.1.3] - 2020-09-21
### Fixed
- Column widths were wrong when multiple different width col-* classes were applied. For example `col-12 col-sm-6 col-lg-4` may rendered a column as 12 wide even above `sm` breakpoint.

## [1.1.2] - 2020-09-17
### Fixed
- Wrong links in Changelog

## [1.1.1] - 2020-09-17
### Fixed
- Fix: `col-N` format classes misbehaved at certain viewport sizes (as opposed to `col-bp-N` classes, where bp is the breakpoint abbr. and N is the col width number)

## [1.1.0] - 2020-09-16
### Added
- New `row-fluid` class to handle special cases with fluid containers. (See readme for description.)

### Fixed
- Side margins misbehaved in certain cases.

## [1.0.2] - 2020-09-15
### Fixed
- Files were included in the npm package that are not needed

## [1.0.1] - 2020-09-15
### Changed
- Recommended installation method changed to use the `bootstrap-responsive-grid` npmjs.com package

## [1.0.0] - 2020-09-15
### Added
- Ability to build `css` files and minify them using npm scripts just like in Bootstrap
- Changelog based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
- FAQ and Known Issues in README.md


## [0.9.0] - 2020-09-14
### Added
- Basic functional package

[Unreleased]: https://github.com/BenceSzalai/bootstrap-responsive-grid/compare/1.1.5...HEAD
[1.1.5]: https://github.com/BenceSzalai/bootstrap-responsive-grid/compare/1.1.4...1.1.5
[1.1.4]: https://github.com/BenceSzalai/bootstrap-responsive-grid/compare/1.1.3...1.1.4
[1.1.3]: https://github.com/BenceSzalai/bootstrap-responsive-grid/compare/1.1.2...1.1.3
[1.1.2]: https://github.com/BenceSzalai/bootstrap-responsive-grid/compare/1.1.1...1.1.2
[1.1.1]: https://github.com/BenceSzalai/bootstrap-responsive-grid/compare/1.1.0...1.1.1
[1.1.0]: https://github.com/BenceSzalai/bootstrap-responsive-grid/compare/1.0.2...1.1.0
[1.0.2]: https://github.com/BenceSzalai/bootstrap-responsive-grid/compare/1.0.1...1.0.2
[1.0.1]: https://github.com/BenceSzalai/bootstrap-responsive-grid/compare/1.0.0...1.0.1
[1.0.0]: https://github.com/BenceSzalai/bootstrap-responsive-grid/compare/0.9.0...1.0.0
[0.9.0]: https://github.com/BenceSzalai/bootstrap-responsive-grid/releases/tag/0.9.0
