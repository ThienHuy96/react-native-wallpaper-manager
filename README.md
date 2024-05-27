# React Native Device Wallpaper Manager

Enhance your Android app with the ability to set wallpapers effortlessly using the React Native New Architecture. This library is optimized for performance, utilizing Kotlin and light-weight threads for a seamless experience.

## Features

- 🐎 **Built with the New Architecture** for better performance and scalability.
- ⚡ **Efficient threading** using light-weight processes.
- 🏎 **Implemented in Kotlin** for a robust and type-safe codebase.

## Getting Started

### Installation

You can add `react-native-device-wallpaper-manager` to your project using npm or yarn:

#### With npm:

```bash
npm install react-native-device-wallpaper-manager
```

#### With yarn:

```bash
yarn add react-native-device-wallpaper-manager
```

### API Reference

#### `setWallpaper` Method

Set the wallpaper of your device with just a few lines of code. The method accepts the following properties:

| Property      | Type   | Description                         | Accepted Values                          |
| ------------- | ------ | ----------------------------------- | ---------------------------------------- |
| `destination` | String | The wallpaper target on the device. | "system", "both", "lock"                 |
| `imageUri`    | String | The URI path to the desired image.  | Remote (http/https) or local (file) URIs |

### Usage Example

Here's a quick example to get you started:

```typescript
import RTNDeviceWallpaper from "react-native-device-wallpaper-manager/js/NativeDeviceWallpaper";

const setWallpaper = async () => {
  await RTNDeviceWallpaper?.setWallpaper(
    "https://your_image_url_here.png",
    "both"
  );
};
```

### Visual Demo

Get a glimpse of what you can achieve with the `react-native-device-wallpaper-manager`:

![Device Wallpaper Manager Demo](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExanF5YzVpZG5ncmNqanp2aW81eW14aTcwdmNyMzBlcmhlcjVjNHduMyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/FpMJDFkj6mNzu600eN/giphy.gif)
