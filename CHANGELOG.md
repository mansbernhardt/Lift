# 2.0.1

- Fixed a bug with forwarding the jar context when using some combinations of nested containers.

# 2.0

- Added support for Swift 4.1 conditional conformance by making `Optional`, `Array` and `Dictionary` to optionally conform to `JarElement`. 
- Conditional conformance makes it easier to build nested jars without explicitly creating jars:
- Previously `let jar: Jar = ["optional": Jar(optional), "array": Jar(array)]` can now be written as: `let jar: Jar = ["optional": optional, "array": array]`.
- Removed all versions of `Jar`' s  `map()` methods as these do not play well with the adding of conditional conformances and you can easily get the same functionally without them.

# 1.0

This is the first public release of the Lift library.
