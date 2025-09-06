# Configuration

The yaml code used on this device which
<a href="https://github.com/SmartHomeGuys/DeskUp-Pro-Controller-RJ12/blob/main/deskup-pro-controller.yaml">can be found here</a>

Was based on this repo: 
<a href="https://github.com/esphome/bluetooth-proxies/blob/main/esp32-generic/esp32-generic-c3.yaml">https://github.com/esphome/bluetooth-proxies/blob/main/esp32-generic/esp32-generic-c3.yaml</a>



We adjusted the following:

## Scan Parameters
Full details of all the properties that can be changed are here:
<a href="https://esphome.io/components/esp32_ble_tracker/#configuration-variables">Configuration variables</a>

With this device we have changed the following values to be different to their defaults. You can change these by adding this code block when editing the yaml in ESPHome.

```
esp32_ble_tracker:
  scan_parameters:
    window: 800ms
    interval: 800ms
```

The original defaults from the repo at the top of this page were these:
```
  window: 30ms
  interval: 320ms
```

However we discovered these settings were not reliable when using FeasyBeacon's or Switchbot Outdoor Climate Meter and the 800ms ones are much more stable. 

You could also decide to change the active: true property to false (to save a bit of device power) however we found this then prevented the Battery Level being read on a Switchbot Outdoor Climate Meter so left this set to true.


## Bluetooth proxy
The bluetooth_proxy section we did not change anything except setting active: true

A list of all its properties can be found here:
<a href="https://esphome.io/components/bluetooth_proxy.html">https://esphome.io/components/bluetooth_proxy.html</a>

