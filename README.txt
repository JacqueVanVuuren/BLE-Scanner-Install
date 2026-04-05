BLE Advert Manufacturing Scanner

This is a phone-installable HTML PWA for Android Chrome.

What it does:
- Scans Bluetooth Low Energy advertisements in the foreground.
- Reads manufacturer data if the browser exposes it.
- Can filter by manufacturer Company ID.
- Can speak decoded data using the phone voice engine.
- Has an IoTI demo decode mode for a simple byte layout:
  byte 0-1 = signed temperature x10, little endian
  byte 2 = production count
  byte 3 = reject count
  byte 4 = status, 0 normal, 1 warning, 2 critical
  byte 5 = machine number

Important:
Web Bluetooth BLE advertisement scanning is experimental in browsers.
For a reliable production scanner, especially background scanning, use a native Android APK.
