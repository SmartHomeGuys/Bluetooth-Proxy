# Setup your Bluetooth Proxy
When you first power on the device it's Led will be solid Yellow this just means it is not connected to your Wi-Fi, once it is the Led will be off.

## Step 1: Connect to Wi-Fi
To do this choose from one of these options:

[Setup using Bluetooth (for Home Assistant users with a Bluetooth proxy)](setup-using-bluetooth.md)

[Setup using USB](setup-using-usb.md)

#### Wi-Fi Troubleshooting
Usually there are no issues with Wi-Fi when using our default firmware but if you do experience any issues with the Wi-Fi connection dropping then below are a few things to try:

- Try relocating the device if its near other sources that can cause Wi-Fi interference on the 2.4GHz band such as a microwave for example.

- Adjust the output power of the device by adopting the device in esphome in home assistant.
  Then gradually increase the Wi-Fi output_power from its default, but dont just put it straight to the maximum as that could potentially cause connection issues too. In the yaml you will find this block:
```
wifi:
  power_save_mode: NONE
  output_power: 9.5dB
```
Documentation for the above is here: https://esphome.io/components/wifi

## Step 2: Add to Home Assistant (optional)
If you missed it in the previous guides, you can add the device so it appears in Home Assistant by following [this guide](add-to-home-assistant.md).  


## Step 3: Configure the device (optional)
If you want to change any of the default settings on the device you need to adopt it in Home Assistant first.

[Adopting in ESPHome Builder](adopting-in-home-assistant.md)

After adoption you can then Configure the device to suit your requirements, we have some examples here.

[Configure the Bluetooth Proxy](../configuration/README.md)
