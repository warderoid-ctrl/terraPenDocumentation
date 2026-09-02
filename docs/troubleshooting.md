# Troubleshooting

!!! tip "Try this first"
    Most problems clear with a power cycle. Switch the terraPen off at the wall, wait
    a few seconds, and switch it back on — see [Restarting](restartTerraPen.md).

## The machine will not move

**It is probably in an alarm state.** FluidNC halts and refuses to move when it stops
trusting its position — most often after a cancelled plot.

Clear it with the **Alarm** button in the interface, or by sending `$X` in the serial
console. Then set your origin again before plotting.

## I cannot reach terrapen.local

`terrapen.local` depends on mDNS, which not every device and network supports.

Use the IP address instead — `http://192.168.0.1` in access point mode, or the
address your router assigned if the terraPen is
[on your own network](connectToPersonalNetwork.md).

## The captive portal is awkward

On macOS and iOS, joining the `terraPen` network opens a cut-down browser panel. It
works, but some controls misbehave.

Open a normal browser window and go to the address directly.

## The terraPen dropped off my Wi-Fi

If it cannot join the network you configured, it gives up after about a minute and
returns to access point mode. Reconnect to the `terraPen` network and check the
settings.

## Lines are broken, faint or torn

This is nearly always **pen height**. Too high and the nib skips; too low and it drags
or tears. Adjust and test on scrap — see
[Your first plot](1stPlot.md#2-fit-the-pen-and-set-its-height).

Also check the pen is tight in the holder and the paper is flat.

## The plot started in the wrong place

The origin was not where you thought. Re-home or re-zero, confirm the readout shows
X0, Y0 before you press play, and check that your G-code was exported with an absolute
origin.

## The pen crashes into the bed

Stop and cut power. This usually means the machine is running the **wrong
configuration for its toolhead** — see
[YAML configuration settings](YAMLConfigurationSettings.md).

## Uploads take forever

Large plots are big files and the transfer is slow. Let it finish rather than
restarting it.

## Still stuck?

Ask on [Discord](https://discord.gg/fEXrmUm5nR). Include your toolhead type, what you
were doing, and anything the serial console printed.
