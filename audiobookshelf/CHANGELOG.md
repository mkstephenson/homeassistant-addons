#### Important: New authentication system was added in [v2.26.0](https://github.com/advplyr/audiobookshelf/releases/tag/v2.26.0). See https://github.com/advplyr/audiobookshelf/discussions/4460 for details.

#### Important: Node.js version updated to 24

### Added

- API keys can authenticate websocket connections by @Vito0912 in #4974

### Fixed

- Server crash decoding invalid filter groups
- Server crash when collapsing sub-series and sorting by author name #4993
- Get series for library endpoint not checking the series belongs to that library

### Updated

- Audible match results now set the explicit flag #5535 by @SharonZhu0122 in #5575
- Server, Docker image, and build scripts now use Node.js 24 by @nichwall in #5578
- API: Library item cover update requires the cover path to be a file already on that library item
- API: Cover and author image cache endpoints require a valid id and positive width/height by @Vito0912
- More strings translated
  - Czech by @CZDanol
  - Norwegian Bokmål by @Mediokris
  - Spanish by @JnBenites
  - Swedish by Daniel Nylander

### Internal

- Initial TypeScript compilation for the server by @nichwall in #5510
- Add ESLint for the server and run it in the unit test workflow in #5578
- Fix ReferenceErrors under strict mode when scanning library directories by @binyaminyblatt in #5586


## New Contributors
* @binyaminyblatt made their first contribution in https://github.com/advplyr/audiobookshelf/pull/5586
* @SharonZhu0122 made their first contribution in https://github.com/advplyr/audiobookshelf/pull/5575

**Full Changelog**: https://github.com/advplyr/audiobookshelf/compare/v2.36.1...v2.37.0