# 2026.1.0
- Updated ESPHome version to 2026.1.2 which introduced Wi-Fi roaming support.
https://esphome.io/changelog/2026.1.0/#wifi-roaming-support
- Removed the Led light and are now using the built in status_led method instead which saves on flash space and reduced the yaml code needed.
- Set the Wi-Fi output_power to 9.5dB as a default which is low but should avoid any Wi-Fi setup issues due and can improve stability, reduce power use, etc. Anyone who needs it to be a higher value can simply adopt the device in ESPHome and adjust it.

# 2025.12.0
- Bump ESPHome version to 2025.11.4

# 2025.11.0
- Switched chip to SeeedStudio XIAO C6

# 2025.9.1
- Bump ESPHome version from 2025.8.2 to 2025.9.0 as it contains more Bluetooth improvements.

# 2025.9.0
- Using the latest ESPHome build 2025.8.2 which contains alot of Bluetooth improvements that have made the device much more stable
- Moved away from the default scan parameter interval: 320ms, window: 30ms and now using 800ms for both which has improved reliability with FeasyBeacon's

# 2025.8.0
- Exposed the LED for control in Home Assistant
- LED displays red when WiFi is not connected, turns off when it is

# 2025.6.1
- First version of a Bluetooth Proxy
