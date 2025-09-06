# Bluetooth Proxy Stick for Home Assistant

## ⚠️ Note this project is a work in-progress right now, expect to be completed by end September 2025. 

<table border="0">
  <tr>
    <td><a href="docs/setup">Setup</a></td>
    <td><a href="docs/configuration">Configure</a></td>
  </tr>
</table>

A Bluetooth (BLE) Proxy for Home Assistant which does not need a cable.

Alot of homes these days have USB sockets everywhere from being on wall power sockets, behind your TV, on your Xbox or a spare socket on a power extension lead, this device lets you plug in the Bluetooth Proxy straight into those for a cable free look. So no more trying to make excess cable look tidy!


### Why do I need a Bluetooth Proxy?



### Specs
- The device itself uses an ESP32-C3 chip that is powered by the built in USB port, no external USB cable is needed to power it.
- The firmware of the Bluetooth Proxy is based on ESPHome and flashed with version 2025.8.2 or higher. This version made the C3 chip alot more stable in our testing.
- Wi-Fi protocol used is 2.4ghz.
- Initial setup of the device to connect it to Wi-Fi can be done using a USB, or Bluetooth (if you use Home Assistant and already have a Bluetooth proxy).


