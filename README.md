# EriaitsevTracker

🌎  #1 tracking tool in the world! 🌎 

1. [Installation](#installation)
2. [Usage](#usage)

## Installation

### CocoaPods

[CocoaPods](https://cocoapods.org) is a dependency manager for Cocoa projects. For usage and installation instructions, visit their website. To integrate EriaitsevTracker into your Xcode project using CocoaPods, specify it in your `Podfile`:

```ruby
pod 'EriaitsevTracker'
```

### Carthage

[Carthage](https://github.com/Carthage/Carthage) is a decentralized dependency manager that builds your dependencies and provides you with binary frameworks. To integrate EriaitsevTracker into your Xcode project using Carthage, specify it in your `Cartfile`:

```ogdl
github "victoryanvc/EriaitsevTracker"
```

### Swift Package Manager

The [Swift Package Manager](https://swift.org/package-manager/) is a tool for automating the distribution of Swift code and is integrated into the `swift` compiler.

Once you have your Swift package set up, adding EriaitsevTracker as a dependency is as easy as adding it to the `dependencies` value of your `Package.swift`.

```swift
dependencies: [
    .package(url: "https://github.com/victoryanvc/EriaitsevTracker.git")
]
```

### Manually

If you prefer not to use any of the aforementioned dependency managers, you can integrate EriaitsevTracker into your project manually.

To use this library in your project manually you may:

1. for Projects, just drag EriaitsevTracker.swift to the project tree
2. for Workspaces, include the whole EriaitsevTracker.xcodeproj

## Usage

Create an `EriaitsevEvent` by passing a dictionary with the desired attributes to be tracked. 

Call `track(event:)` with the event to track it. 

```swift
let params = ["name": "bob"]
let event = Event(params: params)
EriaitsevTracker.shared.track(event)
```

That's it! 🌸

The console should print if the tracking was successful or not, with the given event. 
