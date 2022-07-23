# Change Log

All notable changes to this project will be documented in this file.

# [2.0.0-alpha.1](https://github.com/stalniy/casl/compare/@casl/prisma@1.0.3...@casl/prisma@2.0.0-alpha.1) (2022-07-23)


### Features

* adds custom prisma generator to provide an ability to customize client library ([189ccca](https://github.com/stalniy/casl/commit/189ccca24518562095731c4cd43f4dc1d0cd826a))


### BREAKING CHANGES

* @casl/prisma requires developers to use custom casl generator in their schema.prisma

   **Before**

   No changes required for schema.prisma

   **After**

   ```prisma
    generator client {
      provider = "prisma-client-js"
    }

    generator caslAdapter {
      provider = "node @casl/prisma/generator.js" // <--- this line is important to add!
    }
   ```

## [1.0.3](https://github.com/stalniy/casl/compare/@casl/prisma@1.0.2...@casl/prisma@1.0.3) (2022-07-23)


### Bug Fixes

* **prisma:** allpows to specify not all models inside Subjects helper ([fb9cf8d](https://github.com/stalniy/casl/commit/fb9cf8d3b41f2030e36d2e774731da3540cca55e))
* improved AbilityTuple ([#616](https://github.com/stalniy/casl/issues/616)) ([270446f](https://github.com/stalniy/casl/commit/270446fe7b68bb00a6546d04d6bee88a816a00ff))
* update prisma to version 4 ([#638](https://github.com/stalniy/casl/issues/638)) ([d5abdf1](https://github.com/stalniy/casl/commit/d5abdf1c82b58c8515d2be48d2cf798add5b1e13))

## [1.0.2](https://github.com/stalniy/casl/compare/@casl/prisma@1.0.1...@casl/prisma@1.0.2) (2022-05-29)


### Bug Fixes

* add 'all' to AbilityTuple ([#615](https://github.com/stalniy/casl/issues/615)) ([70025ac](https://github.com/stalniy/casl/commit/70025ac13a8acdf4093d5379961198daf26e9007)), closes [#584](https://github.com/stalniy/casl/issues/584)
* makes sure `WhereInput<T>` resolves to corresponding Prisma model ([9288dcb](https://github.com/stalniy/casl/commit/9288dcb9a6eb91671b23c38454e189cd561af235)), closes [#613](https://github.com/stalniy/casl/issues/613)
* **package:** add repository directory into package.json for all @casl/* packages ([#560](https://github.com/stalniy/casl/issues/560)) ([0ef534c](https://github.com/stalniy/casl/commit/0ef534c9df44816cd64d5142f41621034e5b70db))

## [1.0.1](https://github.com/stalniy/casl/compare/@casl/prisma@1.0.0...@casl/prisma@1.0.1) (2021-10-07)

# 1.0.0 (2021-08-16)


### Bug Fixes

* **prisma:** fix 'isNot' and 'none' condition ([#538](https://github.com/stalniy/casl/issues/538)) ([d3bde31](https://github.com/stalniy/casl/commit/d3bde31b77986b4a99638bd72550d72ce2160200))
* adjusts package tags to improve discoverability ([73e88b0](https://github.com/stalniy/casl/commit/73e88b0a256625b193b2cd9dc4a219f2e1193cbc))
* **prisma:** sets minimum @casl/ability version to 5.3.0 ([55615e4](https://github.com/stalniy/casl/commit/55615e44fa22bfe2b4f2791f6eb218db1df5cfcc))


### Features

* **prisma:** adds prisma integration ([#505](https://github.com/stalniy/casl/issues/505)) ([9f91ac4](https://github.com/stalniy/casl/commit/9f91ac403f05c8fac5229b1c9e243909379efbc6)), closes [#161](https://github.com/stalniy/casl/issues/161) [#161](https://github.com/stalniy/casl/issues/161)


### Performance Improvements

* adds small optimizations in inverted parsing instructions and `toComparable` helper ([32596d1](https://github.com/stalniy/casl/commit/32596d119f26dab09347a0b781a63773c66a3ebc))

# [1.0.0-alpha.2](https://github.com/stalniy/casl/compare/@casl/prisma@1.0.0-alpha.1...@casl/prisma@1.0.0-alpha.2) (2021-05-12)


### Bug Fixes

* adjusts package tags to improve discoverability ([73e88b0](https://github.com/stalniy/casl/commit/73e88b0a256625b193b2cd9dc4a219f2e1193cbc))
* **prisma:** sets minimum @casl/ability version to 5.3.0 ([55615e4](https://github.com/stalniy/casl/commit/55615e44fa22bfe2b4f2791f6eb218db1df5cfcc))

# 1.0.0-alpha.1 (2021-05-10)


### Features

* **prisma:** adds prisma integration ([#505](https://github.com/stalniy/casl/issues/505)) ([9f91ac4](https://github.com/stalniy/casl/commit/9f91ac403f05c8fac5229b1c9e243909379efbc6)), closes [#161](https://github.com/stalniy/casl/issues/161) [#161](https://github.com/stalniy/casl/issues/161)
