# 1. Introduction

Currently (2021 February), Pangle has official Advanced Bidding with Mopub, Ironsource, and MAX, and all of our partners have opened Advanced Bidding to publishers.
However, Pangle still only supports the whitelisted Advanced Bidding. Thus, if you want to use Pangle's Advanced Bidding, please reach out to the Pangle BD to help you apply for the Advanced Bidding whitelist.


## Setup on Pangle

## Setup on Mopub

## Setup on Ironsource

## Setup on MAX


## Environment requirement
- IOS 9.X and higher;
- Xcode 12 and higher;
- Supported architecture: x86-64, armv7, arm64, i386


## Import Pangle SDK through CocoaPods (Recommened):
The simplest way to import the SDK into an iOS project is to use CocoaPods. Open your project's Podfile and add this line to your app's target:

- Note: Import Pangle SDK that the version is higher than v3.4.0.0
```XML
pod 'Ads-Global', '~>3.4.1.1' 
```


- Note: If you wanna import old version of Pangle SDK that the version is lower than v3.4.0.0, as shown below:
```XML
pod 'Bytedance-UnionAD', '~>3.3.6.2'
```



## Download Pangle SDK Manually:
Download and unzip the SDK framework from Pangle Platform directly, and import the following frameworks and bundles into your Xcode project manually:

- `BUAdSDK.framework`
- `BUFoundation.framework`
- `BUAdSDK.bundle`
- `BUVAAuxiliary.framework`

<img src="" />



**Note: When you upgrade the SDK, you need to update all frameworks and bundle files.**


Please make sure that `Copy Bundle Resource` contains `BUAdSDK.bundle`.






### Xcode Compiler Option Settings

#### Add Permissions

Add the parameter `-objc` to `Other Linker Flags` in build settings, and the SDK supports `- all_ load`

##### Detailed Steps:





#### Add Dependency Libraries

Project needs to find Link Binary With Libraries in `TARGETS` - > `Build Phases`, click "+", and then add the following dependent libraries in order.

- StoreKit.framework
- MobileCoreServices.framework
- WebKit.framework
- MediaPlayer.framework
- CoreMedia.framework
- AVFoundation.framework
- CoreTelephony.framework
- SystemConfiguration.framework
- AdSupport.framework
- CoreMotion.framework
- Accelerate.framework
- libresolv.9.tbd
- libc++.tbd
- libz.tbd
- libsqlite3.tbd
- libbz2.tbd
- libxml2.tbd
- libiconv.tbd
- Security.framework


**Note: Add the `ImageIO.framework` if the above dependency library is still reporting errors.**

##### Detailed Steps:



#### Add language configuration








