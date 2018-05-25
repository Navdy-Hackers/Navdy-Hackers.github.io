## How to update HERE Maps

You can update the HERE Maps for display!

### Requirements
* an Android device
* Android developer tools installed on your computer (to have access to `abd`)
* Android device in USB debugging mode

### Instructions
1. Search, download, and install the .apk named: `HERE WeGo Offline Maps GPS v2.0.11480` **Note: Later versions are not working.**
2. Launch the app, go to the sidebar and tap Download Maps
3. Download the offline maps for your region.  (I downloaded USA and Canada, not the whole North America region.  I'm not sure if it matters.)
4. Plug your phone into the computer.
5. Use `adb pull /sdcard/Android/data/com.here.app.maps/files/.here-maps/diskcache-v4` to get the maps on your computer.
   * You might need to replace `/sdcard/` with something like `/storage/emulated/0/` if your phone uses Internal Storage
   * If you're missing your PATH variable for adb, but you still have it downloaded, you could call it like this: `"C:\Users\YOUR_USERNAME_HERE\AppData\Local\Android\Sdk\platform-tools\adb.exe"`
   * The contents of that folder will be copied to wherever your command prompt is open to.
6. Plug your Navdy into the computer.
7. Back up the `.here-maps\diskcache-v4` folder from your Navdy.  Save this somewhere safe, so you can revert in case something goes wrong.
8. Copy the new `diskcache-v4` folder onto your Navdy.
   * Note: I needed to delete the existing files under `diskcache-v4` on my Navdy, to make room for the new ones.

This guide was shamelessly plagarized from [navx2vad's post on xda-developers](https://forum.xda-developers.com/showpost.php?p=76393133&postcount=2)!
