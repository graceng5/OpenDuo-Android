# Open Duo for Android

*其他语言版本： [简体中文](README.zh.md)*

The Agora Android OpenDuo sample app is an open-source demo that integrates video chat into your Android applications using the Agora Video SDK and the Agora Signaling SDK.

With this sample app, you can:

- Login the signaling server
- Inquire whether the calling subscriber is online
- Call each other, join the call, end the call
- Mute/unmute the audio
- Switch the camera

The Agora Video SDK supports iOS/Android/Web. You can find the demos of these platform here:

- [OpenDuo-iOS-Objective-C] (https://github.com/AgoraIO/OpenDuo-iOS-Objective-C)
- [OpenDuo-Web] (https://github.com/AgoraIO/OpenDuo-Web)

## Running the App
**First**, create a developer account at [Agora.io] (https://dashboard.agora.io/signin/), and obtain an App ID.
Update "app/src/main/res/values/strings.xml" with your App ID.

```
<string name="agora_app_id"><#YOUR APP ID#></string>

```

`Currently this project is compatible with the Agora Video SDK 2.1.0 and the Agora Signaling SDK 1.2.1`

**Second**, download the Video SDK and Signaling SDK from [Agora.io SDK] (https://www.agora.io/en/download/). Unzip the downloaded SDK package and copy ***.jar** under **libs** to **app/libs**, **arm64-v8a**/**x86**/**armeabi-v7a** under **libs** to **app/src/main/jniLibs**.

Then, add the following code in the property of the dependence of "app/build.gradle" (included in the sample):

```
  compile fileTree(dir: 'libs', include: ['*.jar'])
```

**Finally**, open the project with Android Studio, connect your Android device, build and run.

Or use `Gradle` to build and run.

## Developer Environment Requirements
- Android Studio 2.0 or later
- Real devices (Nexus 5X or other devices)
- Some emulators have missing functions or performance issues, so real devices are recommended

## Connect Us
- You can find the API documentation at [Document Center] (https://docs.agora.io/en/).
- You can report issues about this demo at [issue] (https://github.com/OpenDuo-Android/issues).

## License
The MIT License (MIT).
