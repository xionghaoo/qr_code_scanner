# QR Code Scanner
[![Build Status](https://dev.azure.com/juliuscanute/spring/_apis/build/status/juliuscanute.qr_code_scanner?branchName=master)](https://dev.azure.com/juliuscanute/spring/_build/latest?definitionId=7&branchName=master)

A QR code scanner that works on both iOS and Android by natively embedding the platform view within Flutter. The integration with Flutter is seamless, much better than jumping into a native Activity or a ViewController to perform the scan.

## iOS Integration
In order to use this plugin, add the following to your Info.plist file:
```
<key>io.flutter.embedded_views_preview</key>
<true/>
```

## Flip Camera (Back/Front)
The default camera is the back camera.
```dart
controller.flipCamera();
```

## Flash (Off/On)
By default, flash is OFF.
```dart
controller.toggleFlash();
```

## Resume/Pause
Pause camera stream and scanner.
```dart
controller.pause();
```
Resume camera stream and scanner.
```dart
controller.resume();
```



# TODO'S:
* iOS Native embedding is written to match what is supported in the framework as of the date of publication of this package. It needs to be improved as the framework support improves.
* In future, options will be provided for default states.
* Finally, I welcome PR's to make it better :), thanks

# Credits
* Android: https://github.com/zxing/zxing
* iOS: https://github.com/mikebuss/MTBBarcodeScanner
* Special Thanks To: LeonDevLifeLog for his contributions towards improving this package.