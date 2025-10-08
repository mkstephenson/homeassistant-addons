#### Important: New authentication system was added in [v2.26.0](https://github.com/advplyr/audiobookshelf/releases/tag/v2.26.0). See https://github.com/advplyr/audiobookshelf/discussions/4460 for details.

### Added

- Book cover search includes "Best" option (searches audible, google & fantlab) by @mikiher in #4716

### Fixed

- OIDC invalid callback URL (incorrect protocol) #4609 by @Vito0912 in #4635
- MultiSelect causing web client to become unresponsive due to duplicate keys #4634 by @nichwall in #4636
- Podcast episodes being downloaded without an audio stream (in #4664)
- UI/UX: Chapter editor overflowing on smaller screen sizes #4652

### Changed

- Book cover search is now async, streams results using websockets by @mikiher in #4716
- Decrease timeout to 10s (from 30s) on all metadata providers by @mikiher in #4716
- UI/UX: Chapter editor does not redirect back after saving changes or deleting all chapters #4650
- More strings translated
  - Arabic by @Salmanegr
  - Chinese (Simplified Han script) by @FiendFEARing
  - Croatian by @biuklija @milotype
  - Czech by @kuci-JK @petr-prikryl @Plazec @Losicek
  - Finnish by @pHamala
  - French by @lolly76
  - German by @Vito0912 @pjope @B0rax
  - Hungarian by @ugyes @Kabika82
  - Norwegian Bokmål by @husjon @PSchaug
  - Persian by @aghorbanmehr
  - Polish by @satanowski @ahetek
  - Portuguese (Brazil) by @jhonthan
  - Romanian by @Hnatiucb @Emdisi00
  - Russian by @GrakovNe @Devastator1979
  - Slovak by @pecer
  - Slovenian by @thehijacker
  - Swedish by @Cotignac
  - Turkish by @icutehunter @smilefate @oersen
  - Ukrainian by @maksim2005UKR

### Internal

- Add a script to build an uncompressed windows executable #2998 by @mikiher in #4729

**Full Changelog**: https://github.com/advplyr/audiobookshelf/compare/v2.29.0...v2.30.0