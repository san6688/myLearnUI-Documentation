```yaml
name: myLearnUI
description: Flutter UI Template to develop cross platform online learning/tutoring apps

# The following line prevents the package from being accidentally published to
# pub.dev using `pub publish`. This is preferred for private packages.
publish_to: 'none' # Remove this line if you wish to publish to pub.dev

version: 1.0.0+1

environment:
  sdk: ">=2.7.0 <3.0.0"

dependencies:
  flutter:
    sdk: flutter
  flutter_launcher_icons: ^0.7.5
  intl: ^0.16.1
  video_player: ^0.10.11+2
  device_preview: ^0.4.7
  cupertino_icons: ^0.1.3

dev_dependencies:
  flutter_test:
    sdk: flutter

flutter_icons:
  android: "launcher_icon"
  ios: true
  image_path: "assets/images/open-book.png"

# The following section is specific to Flutter.
flutter:
  uses-material-design: true
  assets:
    - assets/images/
    - assets/videos/

  fonts:
    - family: Ubuntu
      fonts:
        - asset: assets/fonts/Ubuntu-Light.ttf
        - asset: assets/fonts/Ubuntu-Regular.ttf
        - asset: assets/fonts/Ubuntu-Medium.ttf
        - asset: assets/fonts/Ubuntu-Bold.ttf


```