# Connect via USB-C

You can drive the terraPen from a computer over USB-C instead of over Wi-Fi, using
software such as Lightburn.

!!! tip "terraForge supports USB too"
    [terraForge](terraForge.md) connects over USB serial as well as Wi-Fi, and is
    better behaved than Lightburn for pen work. Consider it first.

## Steps

1. Plug the terraPen into a wall outlet as normal.
2. Connect a USB-C cable between the terraPen and your computer.
3. Find which COM port it appeared on. On Windows, check Device Manager:

    ![Finding the COM port in Device Manager](img/DeviceManagerCOMPort.png)

4. Connect to that port in Lightburn:

    ![Lightburn connected over USB](img/LightburnConnectedTethered.png)

5. Check the serial console for the connection status:

    ![Lightburn console showing a locked machine](img/LightburnConsoleLocked.png)

6. If the machine reports an **alarm** state, send `$X` to clear it:

    ![Clearing the alarm with $X](img/AlarmOff$X.png)

## Known limitations

!!! warning "Tethered control is not fully working"
    Over USB, the **move commands drive the axes incorrectly**, and **pen up / pen
    down does not work correctly**. Use Wi-Fi, or plot from the SD card, for reliable
    results.

For background on connecting Lightburn to FluidNC, see the
[FluidNC Lightburn documentation](http://wiki.fluidnc.com/en/support/senders/lightburn).
