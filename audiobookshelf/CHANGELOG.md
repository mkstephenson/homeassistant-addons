#### Important: New authentication system was added in [v2.26.0](https://github.com/advplyr/audiobookshelf/releases/tag/v2.26.0). See https://github.com/advplyr/audiobookshelf/discussions/4460 for details.

### Added

- Chapter editor tools/enhancements including bulk chapter import & more (see #4384) by @josh-vin in #4384
- Book library sort options for `Progress: Started` and `Progress: Finished` #4540 by @tagmeh in #4575

### Fixed

- Initial page load failing to load library (on token refreshes) #4567 (in #4590)
- Library path folder browser not working on latest Windows 11 (replace `wmic` with `powershell`) #4531 by @sir-wilhelm in #4533
- Podcast itunes id not set on podcasts created from search and podcast matching #4614
- Book match tab last used provider saved in local storage being overriden by itunes when matching a podcast #4615
- Server listening log for ipv6 host by @renesat in #4595
- UI/UX: Podcast match author input not showing the current author value #4617

### Changed

- Podcast episode download requests pass `*/*` in `Accept` header by @renesat in #4596
- Podcast episode downloads always embed meta tags (previously only mp3) (in #4598)
- Remove unnecessary token from HLS playlist files by @laxandrea in #4608
- UI/UX: Changed book library `Progress Updated` sort option label to `Progress: Last Updated`
- UI/UX: Replace SVG icons with material-symbols icon equivalents by @Toby222 in #4552
- UI/UX: Remove unnecessary success toast for podcast episode removed #4606
- More strings translated
  - Belarusian by @i-Nosferatu-i
  - Bulgarian by @jeliozver
  - Chinese (Simplified Han script) by @FiendFEARing
  - Croatian by @biuklija
  - Czech by @kuci-JK
  - Dutch by @matieke
  - German by @Vito0912 @Dalabad @Eragos @B0rax
  - Hungarian by @ugyes @Kabika82
  - Italian by @paolor72 @laxandrea
  - Russian by @renesat
  - Slovenian by @thehijacker
  - Spanish by @idojius86
  - Swedish by @Cotignac @MageSneaky
  - Vietnamese by @phamngocminhhang

## New Contributors
* @laxandrea made their first contribution in https://github.com/advplyr/audiobookshelf/pull/4608
* @renesat made their first contribution in https://github.com/advplyr/audiobookshelf/pull/4596
* @sir-wilhelm made their first contribution in https://github.com/advplyr/audiobookshelf/pull/4533
* @tagmeh made their first contribution in https://github.com/advplyr/audiobookshelf/pull/4575

**Full Changelog**: https://github.com/advplyr/audiobookshelf/compare/v2.28.0...v2.29.0