#### Important: New authentication system was added in [v2.26.0](https://github.com/advplyr/audiobookshelf/releases/tag/v2.26.0). See https://github.com/advplyr/audiobookshelf/discussions/4460 for details.

### Added

- Turkish & Korean language option

### Fixed

- Chapter editor: Play button is still shown next to chapters with invalid start times #4691
- Switching users does not refresh available libraries #4694
- Admin users unable to close sessions for other users #4746
- Custom metadata providers not showing in library edit modal #3820 by @mikiher in #4750
- HLS transcoding fails for AC3/EAC3 codecs #4798 by @Vito0912 in #4808
- UI/UX: Next/prev buttons not shown on item edit modal when opened using "Files" or "Match" context menu item #4718

### Changed

- Increase default access & refresh token expirations. Refresh now 30 days & Access now 1 hour by @Vito0912 in #4756
- Enable OIDC auth auto redirect via query parameter `?autoLaunch=1` on login page by @Yetangitu in #4737
- Improve podcast RSS feed parser to handle feeds not wrapping html in `CDATA` #4757
- Update "Days in a row" stat to not require today by @jamerst in #4770
- Improved error handling for file system ensureDir by @mikiher in #4881
- UI/UX: Rephrase library watcher setting to "Automatically watch ..." #4095 by @mikiher in #4815
- UI/UX: Uploader shows progress indicator #895 by @Vito0912 in #4702
- API: New GET `/search/providers` endpoint to fetch all metadata providers by @mikiher in #4750
- More strings translated
  - Catalan by @celigabon
  - Chinese (Simplified Han script) by @FiendFEARing
  - Croatian by @biuklija @milotype
  - Czech by @Plazec @zendiik
  - Danish by @Andersborrits
  - Estonian by @alehandro112
  - Finnish by @pHamala @phewi
  - French by @dapitch666
  - German by @Blubberland @schoenfeldj @Vito0912 @B0rax
  - Hungarian by @ljaksys @ugyes
  - Italian by @burghy86
  - Korean by @zardkim
  - Lithuanian by @waipit
  - Polish by @pryszczoskor
  - Portuguese (Brazil) by @pmangro @nlqog @ljaksys
  - Romanian by @dinuzauri
  - Russian by @renesat
  - Slovenian by @thehijacker
  - Swedish by @3nm1 @Cotignac
  - Ukrainian by @maksim2005UKR

## New Contributors
* @Yetangitu made their first contribution in https://github.com/advplyr/audiobookshelf/pull/4737
* @jamerst made their first contribution in https://github.com/advplyr/audiobookshelf/pull/4770

**Full Changelog**: https://github.com/advplyr/audiobookshelf/compare/v2.30.0...v2.31.0