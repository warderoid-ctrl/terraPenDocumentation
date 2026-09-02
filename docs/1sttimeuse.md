# First time setup

This page gets your terraPen powered up and connected. Allow about five minutes.

Fit the [stepper toolhead](assembly.md) first if you have not already.

## 1. Connect the power

The power socket is on the controller, **underneath the base board**. Lift the front
of the machine to reach it.

Connect the supplied 12 V adaptor and plug it into the wall.

!!! note "There is no power switch"
    The terraPen turns on as soon as power reaches it. To turn it off, switch off at
    the wall or unplug it. A switched extension lead or a smart plug makes this much
    easier day to day.

## 2. Connect to the terraPen's Wi-Fi

Out of the box the terraPen creates its own access point — it does not join your
network yet.

On your computer, open the Wi-Fi settings and look for:

- **Network name:** `terraPen`
- **Password:** `12345678`

Join it. Your device will warn you that this network has no internet access, which is
expected — you are connecting straight to the machine.

## 3. Open the interface

What happens next depends on your computer:

- **Windows** — a browser page opens by itself, showing the built-in interface.
- **macOS** — a captive portal window opens. **Close it** and use a normal browser
  instead; the portal is a cut-down browser and some controls misbehave in it.

Either way, you can reach the interface directly at:

- [http://192.168.0.1](http://192.168.0.1)
- [http://terrapen.local](http://terrapen.local)

!!! tip "If terrapen.local does not load"
    It relies on mDNS, which some networks and computers do not support. Use the IP
    address instead.

## 4. Put the terraPen on your own network

Working over the access point means your computer has no internet while you plot, so
the next step is to move the terraPen onto your own Wi-Fi.

Follow [Connect to your own Wi-Fi network](connectToPersonalNetwork.md), then come
back here.

## Next steps

- Install [terraForge](terraForge.md) — the recommended way to drive the machine
- Learn the [web interface](terraPenWebUI.md)
- Make something — [Your first plot](1stPlot.md)
