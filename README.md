# choco-allen
Filtering algorithms for Allen's relations

## What's this fork?

This is a fork of the [original repository by the choco team](https://github.com/chocoteam/choco-allen).
Their version uses an outdated and not precisely specified choco version, which prohibits to run their code as-is.

In this repository we updated the code in two steps:
1. We fixed the choco version to the closest version on maven that compiled and required the least API changes (version 4.0.0.a). [See the diff for Tag Choco4.0.0.a](https://github.com/HelgeS/choco-allen/compare/d1ae975...c66da6d)
2. We upgraded choco-solver to the current version 4.10.14. This required some API changes, especially for `IntIterableRangeSet`, and changed behavior in its `removeBetween` method. After our changes the tests pass. [See the diff](https://github.com/HelgeS/choco-allen/compare/c66da6d...9d4ff06)
