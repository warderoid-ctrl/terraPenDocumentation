# Connect via USB-C

The terraPen can be driven over USB-C instead of Wi-Fi.

## With terraForge

USB works well with [terraForge](terraForge.md), including uploading files to the
machine.

1. Plug the terraPen into a wall outlet as normal.
2. Connect a USB-C cable between the terraPen and your computer.
3. In terraForge, open **machine settings** and select **USB** rather than Wi-Fi.
4. Connect.

That is all that is required — jogging, homing, pen control, file upload and plotting
all work over the cable.

!!! tip "Useful when Wi-Fi is awkward"
    A cabled connection avoids network problems entirely, which can be worth it in a
    busy studio or a space with poor Wi-Fi.

## With Lightburn

You can also connect Lightburn over USB, though [terraForge](terraForge.md) is the
better tool for pen work.

1. Find which COM port the terraPen appeared on. On Windows, check Device Manager:

    ![Finding the COM port in Device Manager](img/DeviceManagerCOMPort.png)

2. Connect to that port in Lightburn:

    ![Lightburn connected over USB](img/LightburnConnectedTethered.png)

3. Check the console for connection status:

    ![Lightburn console showing a locked machine](img/LightburnConsoleLocked.png)

4. If the machine reports an **alarm**, send `$X` to clear it:

    ![Clearing the alarm with $X](img/AlarmOff$X.png)

See [Lightburn profiles and settings](LightburnProfilesAndSettings.md) for the
profiles and settings to use.

For background on Lightburn with FluidNC, see the
[FluidNC Lightburn documentation](http://wiki.fluidnc.com/en/support/senders/lightburn).
