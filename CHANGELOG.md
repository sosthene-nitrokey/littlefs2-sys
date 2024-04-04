# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added

- Add `malloc` feature flag. It allows `littlefs` to link to `malloc` and `free` instead of relying on the caller to allocate memory ([#9])
- Add a `software-intrinsics` feature flag, to disable the use of compiler intrinsics when compiling littlefs ([#12][])

# Changed

- upgrade `bindgen` to 0.69.4 and limit symbols to those prefixed with `lfs_` and `LFS_` ([#10])

[#10]: https://github.com/trussed-dev/littlefs2-sys/pull/10
[#12]: https://github.com/trussed-dev/littlefs2-sys/pull/12

## [0.1.7] - 2022-01-26

### Fixed

- Fixed compilation issue caused by other crates also using `bindgen` by selecting the `runtime` feature ([#5])

[#5]: https://github.com/trussed-dev/littlefs2-sys/pull/5
[#9]: https://github.com/trussed-dev/littlefs2-sys/pull/9

[Unreleased]: https://github.com/trussed-dev/littlefs2-sys/compare/0.1.7...HEAD
[0.1.7]: https://github.com/trussed-dev/littlefs2-sys/compare/0.1.6...0.1.7
