# clevertap_flutter

Clevertap plugin (Android/iOS) for Flutter

*Note*: This plugin is still under development, and some APIs might not be available yet. 

## Setup

### Android Project setup:

Add your CleverTap Account ID and CleverTap Token in AndroidManifest.xml of your Android project

### iOS Project setup:

Add your CleverTap Account ID and CleverTap Token in Info.plist of your iOS project

## Usage

```dart
import 'package:clevertap_flutter/clevertap_flutter.dart';
```

PushProfile:

```dart
ClevertapFlutter.pushProfile('TestName', 'test@gmail.com');
```

On User Login:

```dart
 Map<String, dynamic> loginMap = {
    "loginParam1": "Param1",
  };

ClevertapFlutter.onUserLogin(loginMap);
```

Push Event With No Params

```dart
ClevertapFlutter.pushEvent('No Params Test Event');
```

Push Event With Params

```dart
Map<String, dynamic> paramsMap = {
    "version": 2.0,
    "name": "TestName",
  };
ClevertapFlutter.pushEvent('No Params Test Event', paramsMap);
```

## Getting Started

See the `example` directory for a complete sample app using CleverTap Flutter Plugin.
