# @strdr4605/react-native-rename

Rename react-native app with just one command

:warning::warning::warning:
**NOTE:** This package is a fork of [react-native-rename@2.4.1](https://github.com/junedomingo/react-native-rename/tree/99aed0cf788d7e95c481e733de414cb2be76fa64) with several improvements.
- [Validate bundleID to match requirements for Android](https://github.com/junedomingo/react-native-rename/pull/93)
- [Change package name for other java files](https://github.com/junedomingo/react-native-rename/issues/95)

:warning::warning::warning: Probable will be depricated in future if original package will implement these changes  

![react-native-rename](https://cloud.githubusercontent.com/assets/5106887/24444940/cbcb0a58-149a-11e7-9714-2c7bf5254b0d.gif)

> This package assumes that you created your react-native project using `react-native init`.

**Note:** This package does not attempt to properly rename build artifacts such as `ios/build` or Cocoa Pod installation targets. After renaming your project you should clean, build, and reinstall third party dependencies to get it running properly with the new name.

## Installation
```
npm install @strdr4605/react-native-rename -g
```

Switch to new branch first
> better to have back-up

```
git checkout -b rename-app
```

## Usage
```
react-native-rename "<newName>"
# or
npx @strdr4605/react-native-rename "<newName>"
```

> With custom Bundle Identifier (Android only. For iOS, please use Xcode)
```
react-native-rename "<newName>" -b <bundleIdentifier>
```

## Example
```
npx @strdr4605/react-native-rename "Travel App"
```
> With custom Bundle Identifier
```
npx @strdr4605/react-native-rename "Travel App" -b io.github.strdr4605.travelapp
```

<a href="https://www.buymeacoffee.com/strdr4605"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;"  target="_blank"></a>
