# CocoaPodsIssueSample
I have Swift iOS project called `Sample`. `Sample` project embeds framework `SampleKit`. `SampleKit` uses cocoa pods. 
```
platform :ios, '8.0'
use_frameworks!

target 'SampleKit' do
  pod 'Alamofire', '~> 3.0'
end
```
When I run it on simulator it works fine. Whe I run on device it fails to load dlibs

```
dyld: Library not loaded: @rpath/Alamofire.framework/Alamofire
  Referenced from: /private/var/mobile/Containers/Bundle/Application/B3646E19-3239-460D-8304-215A0C2E4F7F/Sample.app/Frameworks/SampleKit.framework/SampleKit
  Reason: image not found
```

Have been banging my head against it hours now. What am I doing wrong ?
