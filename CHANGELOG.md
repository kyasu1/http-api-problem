# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.16.0] - 2020-02-05
### Added
- A changelog
- `ApiError` implements `std::error::Error` if `failure` feature is not activated.

### Changed
- `failure` support must be activated via feature `with-failure`
- If `failure` feature is activated, both `HttpApiProblem` and `ApiError` implement `failure::Fail`, otherwise `std::error::Error`
- Feature `with_warp` became `with-warp`
- Feature `with_actix_web` became `with-actix-web`
- Feature `with_hyper` became `with-hyper`
- Updated `README.md`
