This release brings the 4th beta of NetxtUI:

- Organization feature to edit elements of read lists and collections.
- Ability to edit multiple series and books at the same time, in sequence and in bulk.
- The following will be persisted and restored: filters, sort, and library sub-view
- User settings have been moved in a dedicated user menu
- Feature to toggle poster display (fill/fit)

## Changelog

## 🚀 Features
**komga**
- default to storing HTTP sessions in database ([1eccb04](https://github.com/gotson/komga/commits/1eccb04))

**nextui**
- add user settings to fill poster containers ([85b7514](https://github.com/gotson/komga/commits/85b7514))
- add user menu and relocate some actions into it ([008f3c5](https://github.com/gotson/komga/commits/008f3c5))
- persist/restore library sub-view ([b91a0c4](https://github.com/gotson/komga/commits/b91a0c4))
- persist/restore sort ([4fbbbb0](https://github.com/gotson/komga/commits/4fbbbb0))
- persist/restore non-transient filters ([27cde27](https://github.com/gotson/komga/commits/27cde27))
- edit books in bulk ([27f8a42](https://github.com/gotson/komga/commits/27f8a42))
- edit series in bulk ([bc78536](https://github.com/gotson/komga/commits/bc78536))
- edit multiple series ([45f0cda](https://github.com/gotson/komga/commits/45f0cda))
- edit multiple books ([dcb7c64](https://github.com/gotson/komga/commits/dcb7c64))
- remove series from collection action in multi select bar ([52bca87](https://github.com/gotson/komga/commits/52bca87))
- remove series from collection action in series menu ([2c4a9c1](https://github.com/gotson/komga/commits/2c4a9c1))
- remove books from read list action in multi-select bar ([c5688ab](https://github.com/gotson/komga/commits/c5688ab))
- remove book from read list action in book menu ([2213e69](https://github.com/gotson/komga/commits/2213e69))
- organize collection elements ([19ba5cc](https://github.com/gotson/komga/commits/19ba5cc))
- organize read list elements ([35ef3d7](https://github.com/gotson/komga/commits/35ef3d7))

## 🐛 Fixes
**api**
- prevent concurrent user creation for unclaimed server ([c7397c2](https://github.com/gotson/komga/commits/c7397c2))

**komga**
- publish readlist/collection creation event after database commit ([3ae0def](https://github.com/gotson/komga/commits/3ae0def)), closes [#2434](https://github.com/gotson/komga/issues/2434) [#2496](https://github.com/gotson/komga/issues/2496)

**nextui**
- toggle for overview section not working on chrome mobile ([00444db](https://github.com/gotson/komga/commits/00444db))
- when editing series metadata publisher and language could not be cleared ([48db4f4](https://github.com/gotson/komga/commits/48db4f4))
- properly load vuetify messages for the current locale ([111b857](https://github.com/gotson/komga/commits/111b857)), closes [#2505](https://github.com/gotson/komga/issues/2505)
- clarify wording for age restrictions ([ef1d65e](https://github.com/gotson/komga/commits/ef1d65e)), closes [#2538](https://github.com/gotson/komga/issues/2538)

**webui**
- clarify wording for age restrictions ([978169e](https://github.com/gotson/komga/commits/978169e)), closes [#2538](https://github.com/gotson/komga/issues/2538)

## 🔄️ Changes
**komga**
- ktlint format ([ca1680c](https://github.com/gotson/komga/commits/ca1680c))

**nextui**
- extract common filter logic ([348986f](https://github.com/gotson/komga/commits/348986f))
- move filter panel into dedicated component ([b56fd14](https://github.com/gotson/komga/commits/b56fd14))
- simplify useFilters composable ([c6c0bdd](https://github.com/gotson/komga/commits/c6c0bdd))
- use common action to edit books and series ([69aad4c](https://github.com/gotson/komga/commits/69aad4c))
- relocate types ([44224ed](https://github.com/gotson/komga/commits/44224ed))
- optional props for PosterUpload ([5e96d65](https://github.com/gotson/komga/commits/5e96d65))
- optional model for LockIcon ([435ffec](https://github.com/gotson/komga/commits/435ffec))
- extract i18n message definition ([a8cea1b](https://github.com/gotson/komga/commits/a8cea1b))
- support nested actions for multi selection ([bcaab5f](https://github.com/gotson/komga/commits/bcaab5f))
- remove unused component ([70452ee](https://github.com/gotson/komga/commits/70452ee))
- relocate form components ([61642a1](https://github.com/gotson/komga/commits/61642a1))
- extract poster update logic into composable ([152face](https://github.com/gotson/komga/commits/152face))
- relocate functions ([021d918](https://github.com/gotson/komga/commits/021d918))
- rename composable ([27131be](https://github.com/gotson/komga/commits/27131be))
- reorganize components ([3cdf723](https://github.com/gotson/komga/commits/3cdf723))

**webui**
- replace deprecated api endpoints ([25c67d1](https://github.com/gotson/komga/commits/25c67d1))

**unscoped**
- adjust manifest colors ([78c40fd](https://github.com/gotson/komga/commits/78c40fd))

## 🧪 Tests
**nextui**
- remove failing storybook test ([88264c7](https://github.com/gotson/komga/commits/88264c7))
- update mock data ([4fa0e70](https://github.com/gotson/komga/commits/4fa0e70))

## 🛠  Build
**komga**
- bump icu4j to 79.1 ([1a7c14f](https://github.com/gotson/komga/commits/1a7c14f))
- bump jreleaser to 1.27.0 ([5d5ba73](https://github.com/gotson/komga/commits/5d5ba73))
- bump sqlite-jdbc to 3.54.1.0 ([14406bc](https://github.com/gotson/komga/commits/14406bc))
- fix warning when running jooq tasks ([c677169](https://github.com/gotson/komga/commits/c677169))

**komga-tray**
- remove unused required jdk modules ([1197846](https://github.com/gotson/komga/commits/1197846))

**nextui**
- rerun npm install ([75167e8](https://github.com/gotson/komga/commits/75167e8))

**webui**
- update Browserslist db ([d8a52fd](https://github.com/gotson/komga/commits/d8a52fd))

**unscoped**
- bump gradle to 9.8.2 ([459ad62](https://github.com/gotson/komga/commits/459ad62))

## 🌐 Translation
**komga-tray**
- translated using Weblate (Italian) ([9e93e98](https://github.com/gotson/komga/commits/9e93e98))
- translated using Weblate (Turkish) ([7c72dc5](https://github.com/gotson/komga/commits/7c72dc5))

**nextui**
- translated using Weblate ([b554404](https://github.com/gotson/komga/commits/b554404))
- extract i18n message definition ([8ceabda](https://github.com/gotson/komga/commits/8ceabda))
- extract missing strings ([d90a05c](https://github.com/gotson/komga/commits/d90a05c))

**webui**
- translated using Weblate (Chinese (Simplified Han script)) ([fac9e3c](https://github.com/gotson/komga/commits/fac9e3c))
- translated using Weblate (Korean) ([29461cc](https://github.com/gotson/komga/commits/29461cc))
- translated using Weblate (Turkish) ([1644007](https://github.com/gotson/komga/commits/1644007))

## ⚙️ Dependencies
**ci**
- bump gradle/actions from 6.4.0 to 6.4.1 ([c77240b](https://github.com/gotson/komga/commits/c77240b))

**nextui**
- bump deps ([dea2c5d](https://github.com/gotson/komga/commits/dea2c5d))

**webui**
- bump follow-redirects from 1.16.1 to 1.16.2 in /komga-webui ([bb90668](https://github.com/gotson/komga/commits/bb90668))
- bump node-forge from 1.4.0 to 1.4.2 in /komga-webui ([2e40cf6](https://github.com/gotson/komga/commits/2e40cf6))


## Contributors
We'd like to thank the following people for their contributions:
Automatic translation add-on, EK, Gauthier, Gauthier Roebroeck, Gino Cicatiello, Tarık Yıldız, on9686, tchirou, 無情天