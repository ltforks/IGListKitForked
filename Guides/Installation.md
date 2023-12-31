# Installation

This guide provides details on how to install `IGListKit`.

## CocoaPods

The preferred method of installation for `IGListKit` is using [CocoaPods](https://cocoapods.org/).

In order to use the latest release of the framework, add the following to your `Podfile`:

```ruby
pod 'IGListKit', '~> 4.0'
```

### Using `main`

Alternatively, you can use the latest version from the [`main` branch](https://github.com/Instagram/IGListKit/tree/main). This is what we use at Instagram, so you can be confident that `main` is always stable and reliable.

```ruby
pod 'IGListKit', :git => 'https://github.com/Instagram/IGListKit.git', :branch => 'main'
```

> **Note:** while `main` is stable, it may have breaking changes. Before updating to `main`, be sure to check the [`CHANGELOG`](https://github.com/Instagram/IGListKit/blob/main/CHANGELOG.md) for details on changes.

### Subspecs

With the exception of `macOS` (which currently only supports the diffing algorithm components), using `pod 'IGListKit'` will get you the full library, including the flexible `UICollectionView` system. Learn more about how to get started in our [Getting Started guide](https://instagram.github.io/IGListKit/getting-started.html).

However, if you only want to use the diffing components of this library, then you can use the diffing subspec in your `Podfile`:

```ruby
pod 'IGListKit/Diffing', '~> 4.0'
```

Regardless of whether you only use the diffing components, or the entire library, the imports are the same:

```swift
import IGListKit
```

## Carthage

If using [Carthage](https://github.com/Carthage/Carthage), add the following to your `Cartfile`:

```ogdl
github "Instagram/IGListKit" ~> 4.0
```
