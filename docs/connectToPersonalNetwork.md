# Connect to your own Wi-Fi network

By default the terraPen runs as an access point — you connect to *it*, which means
your device drops off the internet while you plot.

Putting the terraPen on your own network instead lets you browse the web and control
the plotter at the same time.

## Run the setup wizard

1. Connect to the `terraPen` access point and open the interface as usual.
2. Click the **menu** button (H), then **Setup**.
3. Click **Start setup**, then **Continue**.

You now see the current Wi-Fi configuration — access point mode, network name
`terraPen`, and its password. You can change these here if you want to.

To join your own network, set each field in turn and click **Set** after each one.
The field turns green when it is accepted.

| Field | Set it to |
|---|---|
| **Role** | Change from *Access Point* to *WiFi Client* |
| **SSID** | Your network's name |
| **Password** | Your network's password |

![Setting the network SSID](img/Settings SSID.png)

![Setting the network password](img/Settings SSID Password.png)

Then click **Continue**, **Close**, and **Yes** to restart the controller.

## Find it on your network

After restarting, the terraPen joins your Wi-Fi. Reach it at:

- [http://terrapen.local](http://terrapen.local), or
- its IP address, for example `http://192.168.1.145`

If `terrapen.local` does not resolve, check your router's list of connected devices
to find the address it was given.

!!! note "A wrong password is not a disaster"
    If the details are wrong, the controller gives up after about a minute and falls
    back to access point mode. Reconnect to the `terraPen` network and correct them.
