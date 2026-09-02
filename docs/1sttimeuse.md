# First time setup

This page gets your terraPen powered up and connected. Allow about five minutes.

## 1. Connect the power

The power socket is on the controller, **underneath the base board**. Lift the front
of the machine to reach it.

Connect the supplied 12 V adaptor and plug it into the wall.

!!! note "There is no power switch"
    The terraPen turns on as soon as power reaches it. To turn it off, switch off at
    the wall or unplug it. A switched extension lead or a smart plug makes this much
    easier day to day.

When it powers on you may hear the toolhead move and the solenoid click. This is
normal.

## 2. Connect to the terraPen's Wi-Fi

Out of the box the terraPen creates its own Wi-Fi network — it does not join yours yet.

On your phone or computer, open the Wi-Fi settings and look for a network called:

- **Network name:** `terraPen`
- **Password:** `12345678`

Join it. Your device will warn you that this network has no internet access — that is
expected, because you are connecting straight to the machine.

## 3. Open the web interface

What happens next depends on your device:

- **Windows** — a browser window usually opens by itself.
- **macOS and iOS** — a captive portal panel appears. This works, but it is a cut-down
  browser and some controls behave oddly.

For full control, open a normal browser window and go to either:

- [http://terrapen.local](http://terrapen.local)
- [http://192.168.0.1](http://192.168.0.1)

!!! tip "Bookmark whichever one works"
    `terrapen.local` is friendlier, but it relies on mDNS, which some Windows machines
    and some networks do not support. If it does not load, use the IP address.

You should now see the terraPen dashboard. From here you can move the pen carriage and
set the machine's zero position.

!!! note "The layout moves around"
    The interface rearranges itself to fit your screen, so panels may not be where the
    screenshots show them on a phone. The panel names stay the same.

## Next steps

- Learn your way around — [The terraPen web interface](terraPenWebUI.md)
- Get plotting — [Your first plot](1stPlot.md)
- Prefer the terraPen on your own Wi-Fi? — [Connect to a personal network](connectToPersonalNetwork.md)
