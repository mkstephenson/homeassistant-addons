## Changelog

## 🐛 Fixes
**api**
- omit UserDto.ageRestriction instead of returning null ([e3a8cc6](https://github.com/gotson/komga/commits/e3a8cc6))

**epub**
- some TOC may not be parsed correctly ([5fc0b7e](https://github.com/gotson/komga/commits/5fc0b7e))

**kobo**
- proxy raw request body to kobo store ([4a7d9a6](https://github.com/gotson/komga/commits/4a7d9a6)), closes [#2289](https://github.com/gotson/komga/issues/2289)

**koreader**
- also accept application/json on Accept header ([ddfe65d](https://github.com/gotson/komga/commits/ddfe65d))

**opds2**
- incorrect latest series navigation links ([717ef82](https://github.com/gotson/komga/commits/717ef82)), closes [#2285](https://github.com/gotson/komga/issues/2285)
- auth logo issue when using base url ([7c00661](https://github.com/gotson/komga/commits/7c00661)), closes [#2285](https://github.com/gotson/komga/issues/2285)

## 🛠  Build
**docker**
- update base image to Ubuntu 26.04 for amd64 and arm64 ([5d14057](https://github.com/gotson/komga/commits/5d14057))

**webui**
- update Browserslist db ([7e0d680](https://github.com/gotson/komga/commits/7e0d680))

**unscoped**
- update homebrew action ([6c2621b](https://github.com/gotson/komga/commits/6c2621b))

## ⚙️ Dependencies
**ci**
- bump gradle/actions from 5 to 6 ([3ca9806](https://github.com/gotson/komga/commits/3ca9806))

**webui**
- bump @xmldom/xmldom from 0.8.12 to 0.8.13 in /komga-webui ([bb60a79](https://github.com/gotson/komga/commits/bb60a79))
- bump axios from 1.13.5 to 1.15.0 in /komga-webui ([85edd8b](https://github.com/gotson/komga/commits/85edd8b))
- bump follow-redirects in /komga-webui ([63de6aa](https://github.com/gotson/komga/commits/63de6aa))
- bump lodash from 4.17.23 to 4.18.1 in /komga-webui ([b77554f](https://github.com/gotson/komga/commits/b77554f))
- bump @xmldom/xmldom from 0.8.10 to 0.8.12 in /komga-webui ([5620e3f](https://github.com/gotson/komga/commits/5620e3f))
- bump brace-expansion from 1.1.12 to 1.1.13 in /komga-webui ([263d3dd](https://github.com/gotson/komga/commits/263d3dd))

**unscoped**
- bump gradle-git-properties plugin from 2.5.2 to 2.5.7 ([dd9c3fa](https://github.com/gotson/komga/commits/dd9c3fa))


## Contributors
We'd like to thank the following people for their contributions:
Gauthier, Gauthier Roebroeck, James Ward, Óliver García Albertos