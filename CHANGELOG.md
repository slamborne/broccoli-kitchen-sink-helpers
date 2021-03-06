# master

# 0.2.5

* Follow symlinks in `copyRecursivelySync`, `copyPreserveSync`, and `hashTree`
* Update `node-glob` to latest (4.0.5).

# 0.2.4

* Validate that `multiGlob` argument is an array

# 0.2.3

* Speed up `hashStrings` by using `MD5` (instead of `SHA256`).
* Add `symlinkOrCopyPreserveSync` for symlinking with copy fallback on Windows

# 0.2.2

* Make `hashTree` match after `copyRecursivelySync`, by disregarding the
  name of the root directory and not including directory times

# 0.2.1

* Make readdir ordering deterministic

# 0.2.0

* Remove `linkRecursivelySync` & `linkAndOverwrite`

# 0.1.2

* Add `copyRecursivelySync` & `copyPreserveSync`
* Change `linkRecursivelySync` & `linkAndOverwrite` to use
  `copyRecursivelySync` & `copyPreserveTime` respectively. We now refuse
  to overwrite in either of those functions, despite the `linkAndOverwrite`
  name.

# 0.1.1

* In `linkRecursivelySync`, link (broken) symlinks correctly

# 0.1.0

* Initial release
