0.9.4
=====

 - compatible with lts-8.13
 - fix TH deriving for sums
 
0.9.3
=====
  - Support ghc-8.4.1
  - Travis config for ghc-8.2.1
  - SafeCopy instance for Data.List.NonEmpty.NonEmpty

0.9.1
=====

 - fixed tests to work with QuickCheck-2.8.2
 - add SafeCopy instance for Word
 - updates for template-haskell 2.11
 - export some internal TH derivation helpers

0.9.0
=====

This version changes the way `Float` and `Double` are serialized to a
more compact format. Old data should be migrated automatically. As a
result, however, the `Float` and `Double` data serialized by this version can not be read
by older versions of `safecopy`.

This change originated as a modification to the way `cereal` 0.5 serializes `Float` and `Double`.

[https://github.com/GaloisInc/cereal/commit/47d839609413e3e9d1147b99c34ae421ae36bced](https://github.com/GaloisInc/cereal/commit/47d839609413e3e9d1147b99c34ae421ae36bced)

[https://github.com/GaloisInc/cereal/issues/35](https://github.com/GaloisInc/cereal/issues/35)
