# Bluetooth Proxy Stick for Home Assistant

## ⚠️ Note this project is a work in-progress right now, expect to be completed by end Jan 2026. 

<table border="0">
  <tr>
    <td><a href="docs/setup">Setup</a></td>
    <td><a href="docs/configuration">Configure</a></td>
  </tr>
</table>

This is a Bluetooth (BLE) Proxy for Home Assistant which does not need a cable, as it has a built in USB socket.  

<p align="center">
Add Product images here
  <img src="images/HomeAssistant-Discovered-Bluetooth-Devices2.png" height="180px" />
</p>
<p align="center">
  Add ebay url here<a href="    " target="_blank"><img src="images/PurchaseOnEbay-Long3.jpeg" height="90px" /></a>
</p>

A lot of homes these days have USB sockets everywhere from being on wall power sockets, behind your TV, on your Xbox, your internet router or a spare socket on a power extension lead. This device lets you plug in the Bluetooth Proxy straight into those for a cable free look.

Gone are the days trying to make excess cable look tidy!  We have designed it to look good, be as small as possible so it's discreet in your home, and therefore should pass the spouse approval test.

We offer a number of variants on our eBay site:
 - USB-A straight
 - USB-A right angle pointing up
 - USB-A right angle pointing down

Both of the right angle devices make it very discreet when used on wall power sockets that have USB-A ports.


### Why do I need a Bluetooth Proxy?
- A Bluetooth Proxy connects to your Home Assistant server via Wi-Fi allowing you to position it nearer to your Bluetooth devices
- Some hardware like the Home Assistant Green do not have Bluetooth built in, so a proxy can provide it that functionality
- Once you have Bluetooth working on Home Assistant you can integrate Bluetooth devices with it such as Switchbot devices that communicate over Bluetooth
- Many devices you can purchase offer their initial setup via Bluetooth BLE even if they don't communicate using it afterwards. BLE enables very easy setup of devices on Home Assistant with near instant detection of them.
- Extend the range of Bluetooth in your house with multiple proxies strategically positioned.
- With multiple Bluetooth Proxies you can use the <a href="https://github.com/agittins/bermuda">Bermuda</a> or <a href="https://espresense.com/home_assistant">ESPresence</a> integrations in Home Assistant to track Bluetooth devices that move around your home


### Automations you could do
- Once a device that communicates over Bluetooth is added to Home Assistant you can then add it to automations and control it.
- Or using Bermuda you could:
  - Have your Home Assistant dashboard on your phone automatically adjust depending on which room you are in
  - Attach ibeacon trackers to your waste and recycling bins and know if they have been put out for collection or are still sat in their usual spot.
  - Attach an ibeacon to your keys and know which room you left them in
    

### Specs
- We build the Bluetooth Proxy Stick's using only certified components from trusted suppliers to ensure reliability and safe operation.
- The device uses the new ESP32-C6 chip that has 2 processors, which is ideal for Bluetooth Proxies using Wi-Fi.
- The Bluetooth Proxy Stick is powered by the built in USB port, no external USB cable is needed.
- The firmware of the device uses ESPHome and is flashed with version 2025.11.4 or higher (which has Bluetooth stability improvements).
- Wi-Fi protocol used is 2.4ghz.
- Initial setup of the device to connect it to Wi-Fi can be done using USB or Bluetooth BLE (if your Home Assistant instance already has Bluetooth capability).

Want to take control just adopt it in ESPHome and flash any changes you need to it, all the code is available free to use and change on our GitHub site.

