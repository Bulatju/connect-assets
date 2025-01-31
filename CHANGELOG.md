# Changes By Release
## 6.0.2
- mincer upgrade to 2.0.1. (Bulats' version)
- csswring update to 7.0.0.
- postcss update to 8.4.21.
- dev:
- connect update to 3.7.0.
- ejs update to 3.1.8.
- mocha update to 10.2.0.


## 6.0.1
- mincer upgrade to 2.0.1. (fixes connect-assets security warnings)

## 6.0.0
- drop support for Node.js versions older than 6
- mincer upgrade to 2.0.0. (fixes connect-assets security warnings)

## 5.4.1
* Fix denial of service in mime: `1.3.4` -> `1.4.1`

## 5.4.0
* Updates mincer to latest: `1.4.2` -> `1.5.0`

## 5.3.2
* Add noSourceMapProtection option to CLI for generating source maps without the XSSI protection header (the string )]}'\n), thanks to @codynguyen

## 5.3.1
* Add embedMappingComments option to CLI for generating source maps with the CLI, thanks to @codynguyen

## 5.3.0
* Added support for generating source maps with the CLI.

## 5.2.1
* Added more explanation for using the compile option from the CLI.

## 5.2.0
* Updates all core dependencies to the latest:
  * `argparse`: `1.0.2` -> `1.0.7`
  * `csswring`: `3.0.5` -> `4.2.2`
  * `mincer`: `1.3.0` -> `1.4.1`
  * `uglify-js: `2.4.23` -> `2.6.2`
  * `postcss`: `5.0.19` (new dependency)
* Changes `build` option to correctly manage whether the assets are saved to disk
* Adds `bundle` option to manage whether the assets are bundled under a single tag (used to actually be controlled by the `build` option)
* Adds support for inline styles and scripts (`jsInline` and `cssInline`), thanks to @iamjochem

### Upgrade Notes
For the majority of people, the changes to `build` option and the addition of `bundle` option should "just work". However, just providing a `buildDir` will no longer start saving assets to disk; the `build` option must also be enabled.

## 5.1.1
* Fix for compile=true ignoring already built asset (#322), thanks to @dapriett
* Fix for serving source maps, thanks to @inukshuk
