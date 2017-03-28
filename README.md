# Bitrise Step to set iOS `PRODUCT_BUNDLE_IDENTIFIER` setting.

Replaces Xcode's project `PRODUCT_BUNDLE_IDENTIFIER` setting by passing in a new value. This is the recommended way to substitute the bundle identifier instead of modifiying the `CFBundleIdentifier` setting in the `Info.plist` file.

From [Xcode 7 Release Notes](https://developer.apple.com/library/content/documentation/Xcode/Conceptual/RN-Xcode-Archive/Chapters/xc7_release_notes.html):

> The new build setting Product Bundle Identifier (PRODUCT_BUNDLE_IDENTIFIER) is the recommended place to set the Bundle Identifier for a target. The target’s Info.plist should be configured to use this build setting by referencing it as $(PRODUCT_BUNDLE_IDENTIFIER) in the value for the CFBundleIdentifier key.

## How to use this Step

Can be run directly with the [bitrise CLI](https://github.com/bitrise-io/bitrise),
just `git clone` this repository, `cd` into it's folder in your Terminal/Command Line
and call `bitrise run test`.
