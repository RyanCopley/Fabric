Fabric
======
This repository contains CocoaPod for Fabric (https://fabric.io).

### Current versions:
* Fabric.framework v1.1.1
* Crashlytics.framework v2.2.9
* TwitterKit.framework v1.4.0
* MoPub.framework v3.3.0

## Installing
1. Use official Fabric app to configure the components you need
2. Remove all frameworks from project which were added by Fabric app
3. Add pods

  ```ruby
pod 'Fabric', '~> 1.2' # required
pod 'Fabric/Crashlytics', '~> 1.2'
pod 'Fabric/MoPub', '~> 1.2'
pod 'Fabric/Twitter', '~> 1.2'
```

4. Change path in Run Script Build command to:

  `./Pods/Fabric/Fabric.framework/run <your organization API key> <your organization build secret>`

## Known issues

Using `Fabric/MoPub` or `Fabric/Twitter` subpecs result in project failing to build if `use_frameworks!` is set.
