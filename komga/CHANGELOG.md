### Notable Entities
Notable Entities bring a flexible way to store additional metadata at book level. It works similarly to authors in the way you can create any kind of notable entity, and associate it with a list of values.

Komga will fetch the following directly from : Teams, Characters, and Locations.

Note that Notable Entities are only available in Nextui.

### NextUI features
A new toggle has been added in the NextUI Server Settings screen that allows you to configure NextUI as the default UI to be loaded. This is a server-wide setting that will apply to every user.

A link has also been added in the NextUI sidebar to go back to the classic UI, and now the UI switch from the sidebar will always be done in the same window/tab, which is more friendly when used inside a PWA.

The NextUI login screen now supports OAuth2 Login, and some settings to hide the login fields, or perform auto-login, have been added to the Server Settings screen.

### HTTP sessions stored in database
HTTP sessions have been historically stored in memory, which meant that sessions would be lost after a restart. Using the 'remember me' function helped to avoid having to re-login in that case, but it was not the best user experience.

This release brings support to store HTTP sessions in a dedicated SQLite database (to avoid congestion with the main database). For now this is only enabled by default on Docker, and will be rolled out more widely at a later stage.

If you experience any issues with the new setup, you can rollback to in-memory sessions by setting the following environment variable: , or in :

### Maskable Icons for PWA

Maskable icons have been added to the PWA manifest, and should render better on Android when installing the app.
## Changelog

## 🚀 Features
**api**
- use RFC 9457 Problem Detail for v3 api ([9fde491](https://github.com/gotson/komga/commits/9fde491))
- add support for notable entities ([2ee7685](https://github.com/gotson/komga/commits/2ee7685)), closes [#2198](https://github.com/gotson/komga/issues/2198)

**komga**
- support storing http sessions in database ([9ecbb41](https://github.com/gotson/komga/commits/9ecbb41))
- add server settings to switch default webui to nextui ([66a8f6a](https://github.com/gotson/komga/commits/66a8f6a))
- import teams/characters/locations from ComicInfo.xml as notable entities ([6523760](https://github.com/gotson/komga/commits/6523760))

**nextui**
- add maskable icons for Android ([758f6ee](https://github.com/gotson/komga/commits/758f6ee))
- missing posters redirection ([dd57a72](https://github.com/gotson/komga/commits/dd57a72))
- filter books by poster ([b5544b7](https://github.com/gotson/komga/commits/b5544b7))
- media analysis redirection ([10b83e0](https://github.com/gotson/komga/commits/10b83e0))
- add support for oauth2 login ([f6fea94](https://github.com/gotson/komga/commits/f6fea94)), closes [#2403](https://github.com/gotson/komga/issues/2403)
- configure default ui from server settings ([79df485](https://github.com/gotson/komga/commits/79df485))
- add drawer menu link to open classic ui ([764595d](https://github.com/gotson/komga/commits/764595d))
- add support for notable entities ([e19377b](https://github.com/gotson/komga/commits/e19377b))

**webui**
- add maskable icons for Android ([dca0769](https://github.com/gotson/komga/commits/dca0769))
- support opening the app from the /classic url ([6d937d9](https://github.com/gotson/komga/commits/6d937d9))

## 🐛 Fixes
**komga**
- shutdown task processor properly ([a53b53c](https://github.com/gotson/komga/commits/a53b53c))
- koreader hash is not recomputed when book file changed ([91aaca3](https://github.com/gotson/komga/commits/91aaca3)), closes [#2483](https://github.com/gotson/komga/issues/2483)

**koreader**
- support single resource sync format ([908ca07](https://github.com/gotson/komga/commits/908ca07)), closes [#2482](https://github.com/gotson/komga/issues/2482)

**nextui**
- wrap user email on user details page ([94504f9](https://github.com/gotson/komga/commits/94504f9))
- untick comicinfo import of collection/readlist in library creation dialog ([67d37b1](https://github.com/gotson/komga/commits/67d37b1))

**webui**
- open nextui in same tab ([57de2e8](https://github.com/gotson/komga/commits/57de2e8))

## 🏎 Perf
**api**
- do not create session for api key authentication ([b84e3da](https://github.com/gotson/komga/commits/b84e3da))

**komga**
- lazily count items for unpaged queries ([d627244](https://github.com/gotson/komga/commits/d627244))
- add database indices ([71bdd15](https://github.com/gotson/komga/commits/71bdd15))

## 🔄️ Changes
**api**
- remove session management for kosync and kobreader ([e86ecc9](https://github.com/gotson/komga/commits/e86ecc9))

**komga**
- apply ktlint format ([a175e3b](https://github.com/gotson/komga/commits/a175e3b))
- remove unnecessary assertions ([18528ee](https://github.com/gotson/komga/commits/18528ee))
- remove EntityNotFoundException ([64bd38e](https://github.com/gotson/komga/commits/64bd38e))
- relocate classes ([7c77d67](https://github.com/gotson/komga/commits/7c77d67))
- use primary key in string temp table ([36611cc](https://github.com/gotson/komga/commits/36611cc))
- move KoreaderHasher.kt to koreader package ([e4ae2b9](https://github.com/gotson/komga/commits/e4ae2b9))

**nextui**
- remove empty sections ([6dafbdd](https://github.com/gotson/komga/commits/6dafbdd))
- open book reader url using /classic url ([5390a7d](https://github.com/gotson/komga/commits/5390a7d))

## 🧪 Tests
**komga**
- fix overall benchmark setup ([1d1599d](https://github.com/gotson/komga/commits/1d1599d))

## 🛠  Build
**deps**
- bump postcss-selector-parser in /next-ui ([0073cf3](https://github.com/gotson/komga/commits/0073cf3))
- bump source-map-js from 1.2.1 to 1.2.2 in /next-ui ([f5f6459](https://github.com/gotson/komga/commits/f5f6459))
- bump org.jsoup:jsoup from 1.23.1 to 1.23.2 ([e708ba1](https://github.com/gotson/komga/commits/e708ba1))

**deps-dev**
- bump shell-quote from 1.10.0 to 1.12.0 in /next-ui ([519e352](https://github.com/gotson/komga/commits/519e352))

**docker**
- use java 25 for amd64/arm64 images ([a4aa0fa](https://github.com/gotson/komga/commits/a4aa0fa))
- enable storing http sessions in database ([61d0bfb](https://github.com/gotson/komga/commits/61d0bfb))

**komga**
- refactor jooq gradle configuration ([93303e6](https://github.com/gotson/komga/commits/93303e6))

**unscoped**
- update Gradle to 9.8.1 ([3b19ef1](https://github.com/gotson/komga/commits/3b19ef1))

## 🌐 Translation
**komga-tray**
- translated using Weblate (Russian) ([ec923be](https://github.com/gotson/komga/commits/ec923be))

**nextui**
- translated using Weblate (Chinese (Simplified Han script)) ([133d30d](https://github.com/gotson/komga/commits/133d30d))
- translated using Weblate (Japanese) ([9644f27](https://github.com/gotson/komga/commits/9644f27))
- extract strings ([a7909dd](https://github.com/gotson/komga/commits/a7909dd))

**webui**
- translated using Weblate (Japanese) ([c07d4f0](https://github.com/gotson/komga/commits/c07d4f0))

## ⚙️ Dependencies
**ci**
- bump gradle/actions from 6.3.0 to 6.4.0 ([c0cd253](https://github.com/gotson/komga/commits/c0cd253))

**komga**
- bump jimfs to 1.3.2 ([bbfda92](https://github.com/gotson/komga/commits/bbfda92))
- bump archunit to 1.5.1 ([02ec012](https://github.com/gotson/komga/commits/02ec012))
- bump junrar to 8.1.2 ([6b9701b](https://github.com/gotson/komga/commits/6b9701b))
- bump commons-lang3 to 3.21.0 ([ce92c93](https://github.com/gotson/komga/commits/ce92c93))
- bump twelve monkeys to 3.15.3 ([c002f3f](https://github.com/gotson/komga/commits/c002f3f))
- bump sqlite-jdbc to 3.53.4.0 ([e160657](https://github.com/gotson/komga/commits/e160657))

**nextui**
- bump deps ([ef4b79c](https://github.com/gotson/komga/commits/ef4b79c))

**webui**
- bump compression from 1.8.1 to 1.8.2 in /komga-webui ([d88bb70](https://github.com/gotson/komga/commits/d88bb70))
- bump source-map-js from 1.0.2 to 1.2.2 in /komga-webui ([dc677b6](https://github.com/gotson/komga/commits/dc677b6))
- bump shell-quote from 1.10.0 to 1.12.0 in /komga-webui ([42429e1](https://github.com/gotson/komga/commits/42429e1))
- bump joi from 17.13.7 to 17.13.8 in /komga-webui ([c3f21a5](https://github.com/gotson/komga/commits/c3f21a5))
- bump proxy-addr from 2.0.7 to 2.0.8 in /komga-webui ([7d61ff7](https://github.com/gotson/komga/commits/7d61ff7))

**unscoped**
- bump jreleaser to 1.26.0 ([690a5d7](https://github.com/gotson/komga/commits/690a5d7))
- bump ben-manes versions to 0.65.0 ([1338792](https://github.com/gotson/komga/commits/1338792))


## Contributors
We'd like to thank the following people for their contributions:
Felix_SANA, Gauthier, Gauthier Roebroeck, gleb, tkymmm, unagisann