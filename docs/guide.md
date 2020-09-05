# Customization Guide

Learning UI Toolkit designed with standard bottom navigation menu, each page will have own title and extra actions which can be added in title bar right menu.

Follow the below steps to add new screens or customize the existing application.

## Adding new screen

All screens are placed under the path **./lib/screens**. If you want to add more screens create a screen file under the same path which will be composed using the widgets in body section.

## Adding new Menu

As the application designed with Bottom Navigation menu pattern, For adding new menu in bottom navigation bar follow the below steps.

* create instance of *BottomTab* class with title, icon and icon title
* Add the instance in *allTabs* list (menu will be rendered based on the order of the list)
* Refer mockData.dart for the existing menu definition.

## Changing Color Theme

All widgets and fonts inherits color from the theme defined in **main.dart** 

Just update the primarySwatch, primaryColor and accentColor as per your customized UI theme.

```dart
  ./main.dart

 ...
 theme: ThemeData(
        primarySwatch: MaterialColor(0xFFE52D27, color),
        primaryColor: _colorFromHex('#e52d27'),
        accentColor: _colorFromHex('#b31217'),
        ...
        ...
```

## Changing Font Family

App is configured with custom font family *Ubuntu* , with font assets stored under **assets/fonts/** to demo the usage of custom font.

You can easily update your font files under **assets/fonts/** folder  and define the new font family in **pubspec.yaml**

```yaml
  # example:
  fonts:
    - family: Ubuntu
      fonts:
        - asset: assets/fonts/Ubuntu-Light.ttf
        - asset: assets/fonts/Ubuntu-Regular.ttf
        - asset: assets/fonts/Ubuntu-Medium.ttf
        - asset: assets/fonts/Ubuntu-Bold.ttf
```


