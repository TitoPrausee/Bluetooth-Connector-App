# Bluetooth Connector App 📱🔗

The Bluetooth Connector App is an advanced iOS application designed to manage Bluetooth connections seamlessly and to interact with connected devices using voice commands. Built with Swift and utilizing CoreBluetooth for Bluetooth connectivity and the Speech framework for real-time voice recognition, this app offers a hands-free experience for interacting with various Bluetooth-enabled devices.

## Features 🌟

- **Bluetooth Device Discovery:** Quickly locate and display nearby Bluetooth devices.
- **Connection Management:** Easily connect to and disconnect from devices directly through the app.
- **Voice Commands:** Use voice commands to interact with connected devices, enhancing the user experience.
- **User-Friendly Interface:** An intuitive interface makes it straightforward to access all features, suitable for all user levels.

## Prerequisites 🛠️

Before using the app, ensure your device meets the following requirements:
- iOS 13.0 or higher
- Bluetooth enabled

## Configuring Info.plist for Permissions 📄

To use Bluetooth and microphone features, you must configure your app's `Info.plist` to request the necessary permissions from the user:

- **Privacy - Bluetooth Peripheral Usage Description (NSBluetoothPeripheralUsageDescription):**
  This permission is required to discover, connect, and interact with Bluetooth peripherals. Add the following entry to your `Info.plist`:

  ```xml
  <key>NSBluetoothPeripheralUsageDescription</key>
  <string>Our app uses Bluetooth to find, connect, and communicate with nearby devices.</string>

Privacy - Microphone Usage Description (NSMicrophoneUsageDescription):
This permission is needed to receive voice commands through the microphone. Add the following entry to your Info.plist:
  ```xml
    <key>NSMicrophoneUsageDescription</key>
    <string>Our app uses the microphone to allow voice commands for controlling connected devices.</string>
