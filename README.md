# AJMessage

[![Language](https://img.shields.io/badge/Swift-4.2-orange.svg)]()
[![CI Status](https://img.shields.io/travis/ajijoyo/AJMessage.svg?style=flat)](https://travis-ci.org/ajijoyo/AJMessage)
[![Version](https://img.shields.io/cocoapods/v/AJMessage.svg?style=flat)](https://cocoapods.org/pods/AJMessage)
[![License](https://img.shields.io/cocoapods/l/AJMessage.svg?style=flat)](https://cocoapods.org/pods/AJMessage)
[![Platform](https://img.shields.io/cocoapods/p/AJMessage.svg?style=flat)](https://cocoapods.org/pods/AJMessage)

## Example

![demo](https://github.com/ajijoyo/AJMessage/blob/master/Demo/demo.gif)

To run the example project, clone the repo, and run `pod install` from the Example directory first.

## Requirements

```
XCode 10.1
Swift 4.2
```

## Installation

AJMessage is available through [CocoaPods](https://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod 'AJMessage'
```
## Used

Simple used
```swift
AJMessage.show(title: "This is title", message: "message for description",position:.top).onHide {
print("did dissmiss")
}
```

customize config

for spesific view present
```swift
let config = AJMessageConfig()
/**
config.titleFont 
*/

AJMessage.show(title: "This is title", message: "message for description", config: config)
```

for global view present
just set `AJMessageConfig.shared` on `didFinishLaunchingWithOptions` 
```swift
let config = AJMessageConfig.shared
/**
config.titleFont 
*/
```

## Author

ajijoyo, self.ajiejoy@gmail.com

## License

AJMessage is available under the MIT license. See the LICENSE file for more info.
