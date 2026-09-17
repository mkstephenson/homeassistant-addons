This release brings the 2nd beta of NextUI. New features include:
- Metadata edition for series and book (single item only for now)
- Edit Collection and Read list information (not yet re-arranging elements)
- Add to collection and Add to read list dialogs
- In the Import Books screen, the dialog to see the book details, or to compare a book for upgrade
## Changelog

## 🚀 Features
**api**
- support image caching for transient book pages ([5e4637d](https://github.com/gotson/komga/commits/5e4637d))
- return a ProblemDetail on MaxUploadSizeExceededException ([352cf75](https://github.com/gotson/komga/commits/352cf75))
- allow listing public settings ([6f39abc](https://github.com/gotson/komga/commits/6f39abc))
- allow sorting for getCollections API ([a5b252d](https://github.com/gotson/komga/commits/a5b252d))

**komga-tray**
- add tray menu to open nextui ([50094a1](https://github.com/gotson/komga/commits/50094a1))

**nextui**
- display book details in import book table ([882557c](https://github.com/gotson/komga/commits/882557c))
- add series and book links in history table ([e98fd4c](https://github.com/gotson/komga/commits/e98fd4c))
- use a button to select series in import books table ([9772f94](https://github.com/gotson/komga/commits/9772f94))
- compare books in book import table ([249105e](https://github.com/gotson/komga/commits/249105e))
- edit series fields when editing oneshot book ([22ab95c](https://github.com/gotson/komga/commits/22ab95c))
- edit single series dialog ([6f911d7](https://github.com/gotson/komga/commits/6f911d7))
- show series attributes on book view for oneshots ([f643ba3](https://github.com/gotson/komga/commits/f643ba3))
- edit single book dialog ([58322a3](https://github.com/gotson/komga/commits/58322a3))
- add external link indicator on announcement cards, and wrap title ([6001521](https://github.com/gotson/komga/commits/6001521))
- add external link indicator on release cards ([457de01](https://github.com/gotson/komga/commits/457de01))
- add chevron icon on touch devices when overview sections are links ([169e1a4](https://github.com/gotson/komga/commits/169e1a4))
- remove underline links on touch devices ([b719887](https://github.com/gotson/komga/commits/b719887))
- support for RTL locales ([376f104](https://github.com/gotson/komga/commits/376f104))
- display error count on tabs in read list edit dialog ([c210b9b](https://github.com/gotson/komga/commits/c210b9b))
- display error count on tabs in collection edit dialog ([6bf5375](https://github.com/gotson/komga/commits/6bf5375))
- rearrange library creation/edition dialog ([c4eafa2](https://github.com/gotson/komga/commits/c4eafa2))
- add v-ktooltip directive ([702601c](https://github.com/gotson/komga/commits/702601c))
- add KTooltip component ([0881dde](https://github.com/gotson/komga/commits/0881dde))
- support pasting cover images from clipboard ([579edce](https://github.com/gotson/komga/commits/579edce)), closes [#1597](https://github.com/gotson/komga/issues/1597)
- edit read list action ([afc57a7](https://github.com/gotson/komga/commits/afc57a7))
- edit collection action ([f3cb447](https://github.com/gotson/komga/commits/f3cb447))
- support unpacking API error message from ProblemDetail ([3e8e171](https://github.com/gotson/komga/commits/3e8e171))
- add to collection action ([d55a443](https://github.com/gotson/komga/commits/d55a443))
- add to read list action ([f22f57d](https://github.com/gotson/komga/commits/f22f57d))

## 🐛 Fixes
**api**
- missing restrictions on some readlist endpoints ([478dc8b](https://github.com/gotson/komga/commits/478dc8b))

**nextui**
- use querycache.refresh instead of fetch ([e008682](https://github.com/gotson/komga/commits/e008682))
- correct toolbar alignment ([785e99c](https://github.com/gotson/komga/commits/785e99c))
- disallow book upgrade selection for oneshot series ([2e444a8](https://github.com/gotson/komga/commits/2e444a8))
- rework edit dialog spacing ([48a92a6](https://github.com/gotson/komga/commits/48a92a6))
- better handling of dialog callback ([401676f](https://github.com/gotson/komga/commits/401676f))
- use square tabs ([4cb2b47](https://github.com/gotson/komga/commits/4cb2b47))
- missed updates from SSE ([f41c069](https://github.com/gotson/komga/commits/f41c069))
- do not prepend on deck book number with # on series view ([f2d1770](https://github.com/gotson/komga/commits/f2d1770)), closes [#2418](https://github.com/gotson/komga/issues/2418)
- better tooltips on mobile ([298a1e2](https://github.com/gotson/komga/commits/298a1e2))
- properly refresh posters upon receiving sse ([d675304](https://github.com/gotson/komga/commits/d675304))
- use normal density for the read list import file upload component ([06501da](https://github.com/gotson/komga/commits/06501da))
- user hasRole default to false instead of undefined ([0345f13](https://github.com/gotson/komga/commits/0345f13))
- don't try to retrieve announcements if the user is not admin ([1d4e933](https://github.com/gotson/komga/commits/1d4e933))
- use menu icon for navigation drawer on mobile ([174ce65](https://github.com/gotson/komga/commits/174ce65))
- card text would be cut off short ([0c044e2](https://github.com/gotson/komga/commits/0c044e2))

## 🏎 Perf
**nextui**
- only load current locale ([c5ff5db](https://github.com/gotson/komga/commits/c5ff5db))

## 🔄️ Changes
**nextui**
- use querycache instead of reactive queries in global error handler ([fe215e4](https://github.com/gotson/komga/commits/fe215e4))
- remove unnecessary refetch ([e8cc58a](https://github.com/gotson/komga/commits/e8cc58a))
- use createGlobalState for singleton composables ([d4d8494](https://github.com/gotson/komga/commits/d4d8494))
- normalize stale time ([cc8b857](https://github.com/gotson/komga/commits/cc8b857))
- remove console output ([5081b67](https://github.com/gotson/komga/commits/5081b67))
- extract logic in app releases query into composable ([ae3fcf8](https://github.com/gotson/komga/commits/ae3fcf8))
- untangle logic in libraries and client settings queries ([89cd951](https://github.com/gotson/komga/commits/89cd951))
- use querycache instead of reactive queries in navigation guard ([1411b65](https://github.com/gotson/komga/commits/1411b65))
- move pinia colada query to the main context for useBooks ([e204543](https://github.com/gotson/komga/commits/e204543))
- move pinia colada query to the main context for ImportReadlistTable ([29184d1](https://github.com/gotson/komga/commits/29184d1))
- move pinia colada query to the main context ([661a5bf](https://github.com/gotson/komga/commits/661a5bf))
- use renderless component in TransientBooksTable ([c9648e9](https://github.com/gotson/komga/commits/c9648e9))
- move util functions to functions directory ([ae1fadb](https://github.com/gotson/komga/commits/ae1fadb))
- extract error count into composable ([bf521d5](https://github.com/gotson/komga/commits/bf521d5))
- small fixes following openapi updates ([b8c2f9b](https://github.com/gotson/komga/commits/b8c2f9b))
- replace cardTextClass with cardTextProps for dialogs ([42f2aad](https://github.com/gotson/komga/commits/42f2aad))

## 🧪 Tests
**nextui**
- update optimizeDeps ([7322c4e](https://github.com/gotson/komga/commits/7322c4e))
- fix msw mocks ([2cf933a](https://github.com/gotson/komga/commits/2cf933a))

## 🛠  Build
**chromatic**
- ignore dependabot ([234b302](https://github.com/gotson/komga/commits/234b302))

**deps**
- bump qs from 6.15.3 to 6.16.0 in /next-ui ([a2cf953](https://github.com/gotson/komga/commits/a2cf953))

**deps-dev**
- bump vitest from 4.1.10 to 4.1.11 in /next-ui ([fa4d1f3](https://github.com/gotson/komga/commits/fa4d1f3))
- bump @humanfs/node from 0.16.6 to 0.16.8 in /next-ui ([f9c4688](https://github.com/gotson/komga/commits/f9c4688))

**nextui**
- rework i18n handling to remove empty files ([2dbbaf0](https://github.com/gotson/komga/commits/2dbbaf0))
- validate translations ([97c0845](https://github.com/gotson/komga/commits/97c0845))
- add unhead ([094daea](https://github.com/gotson/komga/commits/094daea))
- generate valibot schemas from openapi ([0909538](https://github.com/gotson/komga/commits/0909538))
- upgrade Vuetify to 4.2.0 ([bb29ff4](https://github.com/gotson/komga/commits/bb29ff4))
- configure throwOnError for the openapi generator ([48e56a6](https://github.com/gotson/komga/commits/48e56a6))

**webui**
- update Browserslist db ([98ee3a8](https://github.com/gotson/komga/commits/98ee3a8))

## 📝 Documentation
**nextui**
- bump deps ([e209a39](https://github.com/gotson/komga/commits/e209a39))

**openapi**
- expose sort parameter for getReadLists API ([fac2f15](https://github.com/gotson/komga/commits/fac2f15))

**unscoped**
- add LLM/AI contribution guidelines ([6b4397f](https://github.com/gotson/komga/commits/6b4397f))
- create SECURITY.md ([c0135eb](https://github.com/gotson/komga/commits/c0135eb))

## 🌐 Translation
**komga-tray**
- translated using Weblate (Italian) ([db36d3b](https://github.com/gotson/komga/commits/db36d3b))
- translated using Weblate (Malayalam) ([2d6f43f](https://github.com/gotson/komga/commits/2d6f43f))
- translated using Weblate (Vietnamese) ([ca18d8a](https://github.com/gotson/komga/commits/ca18d8a))

**nextui**
- translated using Weblate (Chinese (Simplified Han script)) ([01bd27d](https://github.com/gotson/komga/commits/01bd27d))
- translated using Weblate ([17d6fac](https://github.com/gotson/komga/commits/17d6fac))
- translated using Weblate (Korean) ([5c2b620](https://github.com/gotson/komga/commits/5c2b620))
- translated using Weblate (French) ([0167fd8](https://github.com/gotson/komga/commits/0167fd8))
- translated using Weblate ([f65a56e](https://github.com/gotson/komga/commits/f65a56e))
- translated using Weblate ([47941a8](https://github.com/gotson/komga/commits/47941a8))
- translated using Weblate ([9008a85](https://github.com/gotson/komga/commits/9008a85))
- translated using Weblate ([142c347](https://github.com/gotson/komga/commits/142c347))
- translated using Weblate ([81ee1f1](https://github.co ...