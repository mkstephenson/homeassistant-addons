#### Important: New authentication system was added in [v2.26.0](https://github.com/advplyr/audiobookshelf/releases/tag/v2.26.0). See https://github.com/advplyr/audiobookshelf/discussions/4460 for details.

### Added

- Server setting to allow a whitelist of CORS origins by @Vito0912 in #4557

### Fixed

- Server crash when transcode requests are made to the direct play endpoint #4555 (in #4565)
- OIDC auto-register still creating a user when groupclaim is invalid #4563
- OIDC callback URL validation

### Changed

- More strings translated
  - Belarusian by @i-Nosferatu-i
  - Chinese (Simplified Han script) by @FiendFEARing
  - Croatian by @biuklija
  - Estonian by @alehandro112
  - French by @ThoDon
  - German by @Vito0912 @numerfolt @LaurinSorgend
  - Hindi by @ashishwadekar
  - Norwegian Bokmål by @Erbros
  - Russian by @NickSkier
  - Ukrainian by @Maksim2005UA2

**Full Changelog**: https://github.com/advplyr/audiobookshelf/compare/v2.27.0...v2.28.0