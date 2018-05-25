## How to update HERE Maps

You can update the HERE Maps for display.  An Android device is required.

1. Install the .apk named: `HERE WeGo Offline Maps GPS v2.0.11480` **Note: Later versions are not working.**
2. Download the offline maps for your region.
3. Plug your phone into the computer.
4. Use `adb pull /sdcard/Android/data/com.here.app.maps/files/.here-maps/diskcache-v4` to get the maps on your computer.  (You might need to replace `/sdcard` if your phone uses Internal Storage)
5. Plug your Navdy into the computer.
6. Back up the `diskcache-v4` folder from your Navdy.  Save this somewhere safe, so you can revert in case something goes wrong.
7. Copy the new `diskcache-v4` folder onto your Navdy.
