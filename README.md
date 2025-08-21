# XC26-Sourcery

## Package Creation

This package was created using the following steps:

1. Initialize a new Swift package:
   ```
   swift package init
   ```
2. Add Sourcery as a dependency:
   ```
   swift package add-dependency https://github.com/krzysztofzablocki/Sourcery.git --branch master
   ```

## Build Error Summary

When running the following command:

```
swift package --allow-writing-to-package-directory sourcery-command
```

we encounter this error:

```
error: the library 'SwiftBuildSupport' requires macos 13.0, but depends on the product 'SwiftBuild' which requires macos 14.0; consider changing the library 'SwiftBuildSupport' to require macos 14.0 or later, or the product 'SwiftBuild' to require macos 13.0 or earlier.
error: the library 'SwiftBuildSupport' requires macos 13.0, but depends on the product 'SWBBuildService' which requires macos 14.0; consider changing the library 'SwiftBuildSupport' to require macos 14.0 or later, or the product 'SWBBuildService' to require macos 13.0 or earlier.
error: the library 'SwiftBuildSupport' requires macos 13.0, but depends on the product 'SwiftBuild' which requires macos 14.0; consider changing the library 'SwiftBuildSupport' to require macos 14.0 or later, or the product 'SwiftBuild' to require macos 13.0 or earlier.
error: the library 'SwiftBuildSupport' requires macos 13.0, but depends on the product 'SWBBuildService' which requires macos 14.0; consider changing the library 'SwiftBuildSupport' to require macos 14.0 or later, or the product 'SWBBuildService' to require macos 13.0 or earlier.
error: fatalError
```
