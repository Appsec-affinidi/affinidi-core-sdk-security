# release 1.6.1 (2022-10-27)
* Fix Security Vulnerabilities by patching `xmldom`
## release 1.6.0 (2022-09-06)
* upgraded to npm 8;
* added `overrides` field to override vulnerable `node-forge` sub dependency(npm version >= 8.10.x);
* fixed typing issues.

## 1.5.1 (2022-08-18)
* fixed `package.json` module after refactored build process

## 1.5.0 (2022-08-01)
* added `LegacyVCV1Subject`

## 1.4.2 (2021-08-30)

Improved types

## 1.4.0 (2021-07-01)

* Added support for "proofValue" field in "proof" entry of the VC
* SignSuite now accepts optional public key for signing (for BBS+ signing process)
* Added tests for BBS+ validation

## 1.3.0

### Improvements

* Reorganized dependencies

## 1.2.0

### Improvements

- Adds the concept of a presentation submission to the `VPV1Unsigned` type and its correlated `buildVPV1Unsigned` function. This is in support of the [presentation-exchange spec presentation submissions](https://identity.foundation/presentation-exchange/#presentation-submissions).

## 1.1.1

### Improvements

- Protect against malleable VCs and VPs
  - `buildVCV1`, `validateVCV1`, and `validateVPV1` now _throws_ when the VC's id is not an absolute URI
  - `buildVCV1Skeleton` and `buildVCV1Unsigned` now _warns_ when VC's id is not an absolute URI
  - `buildVPV1` and `buildVPV1Unsigned` now _warns_ if an id is not provided and _throws_ if an id is provided but not an absolute URI

## 1.0.0

- Initial release
