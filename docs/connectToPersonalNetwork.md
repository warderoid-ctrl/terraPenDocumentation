# Connect to your own Wi-Fi network

By default the terraPen runs as an access point — you connect to *it*, which means
your computer drops off the internet while you plot.

Putting the terraPen on your own network fixes that, and is how you will normally use
it.

## 1. Enter your network details

Connect to the `terraPen` access point and open the interface, then set your network
name and password in the controller settings.

![Setting the network SSID](img/Settings SSID.png)

![Setting the network password](img/Settings SSID Password.png)

Click **Set** after each field.

## 2. Restart the controller

Select the **ESP3D** tab and click the red **power** icon to reset — see
[Restarting the terraPen](restartTerraPen.md).

## 3. Check whether it worked

This is the quick way to tell, without hunting through router settings:

**Look at your computer's list of available Wi-Fi networks.**

| What you see | What it means |
|---|---|
| `terraPen` has **disappeared** | It worked. The plotter is on your network. |
| `terraPen` is **still there** | It failed and has fallen back to access point mode. Reconnect and check the details. |

!!! note "Failing is harmless"
    If the details are wrong, the controller gives up and returns to access point
    mode. Nothing is broken — reconnect to `terraPen` and try again.

## 4. Reconnect

Put your computer back on your normal Wi-Fi network, then reach the plotter with
either:

- **[terraForge](terraForge.md)** — recommended
- A browser at [http://terrapen.local](http://terrapen.local)

If `terrapen.local` does not resolve, check your router for the address it assigned,
for example `http://192.168.1.145`.
