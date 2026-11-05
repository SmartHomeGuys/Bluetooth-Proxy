### Notes on how to flash the latest version to a new device for a customer
- In a Chrome browser go to: https://smarthomeguys.github.io/Bluetooth-Proxy/Setup.html
- Choose the 'Install' option, connect it to Wi-Fi
- Test the device.
- After testing, reflash the device again using the 'Install' option but this time 'Skip' adding it to Wi-Fi.
- Unplug and package up for shipping.
- Remove the 'Bluetooth Proxy' device from Home Assistant so it does not exist as a device under integrations or under ESPHome Builder or Unify.

### Notes on how to release a new version
- Make code changes locally (avoiding using Git) on a development version of a device.
- No need to worry about version numbers at this point.

- Once development is complete update the local Git repo's bluetooth-proxy.yaml & bluetooth=proxy-to-flash.yaml with the code chnages and a new version number.

- Update CHANGELOG.md
- Commit and push to GitHub.
- Wait 1 minute for any local GitHub cached files to expire from cache.


- Run powershell command BuildBluetoothProxyRelease.ps1 found in c:\[userfolder]\esphome
- This will build a firmware version.

  - In VSCode the 2 bin files and a firmware.md5 file should already be listed under commits. 
  - Update the version number in the manifest.json file
  - Now check these 4 updated files into Git


- In the GitHub repo add a version.

- Users Home Assistant clients should now start saying an updated version is available to install.
