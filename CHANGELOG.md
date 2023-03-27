# Changelog

Following panolint version 0.1.6, we stopped formally releasing new panolint versions in favor of continually releasing and incorporating the latest iteration of this code.

This file documents notable changes to the project through version 0.1.6. The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.1.6] - 2022-10-19

### Changed

- Disabled `Rails/I18nLocaleTexts`
- Removed several redundant configurations

## [0.1.5] - 2022-07-19

### Changed

- Configured `Layout/LineContinuationSpacing` to use `EnforcedStyle: no_space`

## [0.1.4] - 2021-11-29

### Changed

- The `rubocop.yml` file renamed to `panolint-rubocop.yml`.
- Skip RuboCop in node_modules/ directory

## [0.1.3] - 2021-04-22

### Added

- Dependabot automation

### Changed

- Enable all new cops by default
- Explicitly enabled rules:
  - `Layout/EmptyLinesAroundAttributeAccessor`
  - `Layout/SpaceAroundMethodCallOperator`
  - `Style/ExponentialNotation`
  - `Style/SlicingWithRange`
  - `Lint/DeprecatedOpenSSLConstant`
  - `Lint/MixedRegexpCaptureTypes`
  - `Style/RedundantRegexpCharacterClass`
  - `Style/RedundantRegexpEscape`
  - `Lint/DuplicateElsifCondition`
  - `Style/ArrayCoercion`
  - `Style/CaseLikeIf`
  - `Style/HashAsLastArrayItem`
  - `Style/RedundantFileExtensionInRequire`
- Explicitly disabled rules:
  - `Gemspec/RequiredRubyVersion`
  - `RSpec/MultipleMemoizedHelpers`

## [0.1.2] - 2020-04-10

### Changed

- The `panolint.yml` file renamed to `rubocop.yml`.
- Add `brakeman` and instructions for running it.

## [0.1.1] - 2020-04-10

### Changed

- Explicitly ignore the `Naming/FileName` rule on `.overcommit/Gemfile` files.
- Change the config name from `.rubocop.yml` to `panolint.yml`.

## [0.1.0] - 2020-04-09

### Added

- Initial release. 🎉

[unreleased]: https://github.com/panorama-ed/panolint/compare/v0.1.3...HEAD
[0.1.6]: https://github.com/panorama-ed/panolint/compare/v0.1.5...v0.1.6
[0.1.5]: https://github.com/panorama-ed/panolint/compare/v0.1.4...v0.1.5
[0.1.4]: https://github.com/panorama-ed/panolint/compare/v0.1.3...v0.1.4
[0.1.3]: https://github.com/panorama-ed/panolint/compare/v0.1.2...v0.1.3
[0.1.2]: https://github.com/panorama-ed/panolint/compare/v0.1.1...v0.1.2
[0.1.1]: https://github.com/panorama-ed/panolint/compare/v0.1.0...v0.1.1
[0.1.0]: https://github.com/panorama-ed/panolint/compare/45c38b...v0.1.0
