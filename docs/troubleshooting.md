# Troubleshooting

!!! tip "Try this first"
    Most problems clear with a power cycle. Switch the terraPen off at the rear
    right, wait a few seconds, and switch it back on — see
    [Restarting](restartTerraPen.md). Home the machine afterwards.

## The machine will not move

**It is probably in an alarm state.** FluidNC halts and refuses to move when it stops
trusting its position — most often after an aborted plot.

1. Clear the alarm — the alarm control in [terraForge](terraForge.md), or `$X` in the
   console.
2. [Home the machine](1stPlot.md#2-home-the-machine) again.

If it still will not move, switch the terraPen off at the rear right, bring it back
up, and home it.

!!! tip "Avoid this next time"
    Aborting a plot is what causes it. **Pause** instead — the machine stops safely
    and you can resume, with no alarm and no re-homing. See
    [pause first](startingAplot.md#stopping-a-plot-pause-first).

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
or tears.

Because neither the bed nor the paper is perfectly flat, set Z zero fractionally
*into* the paper rather than exactly level — the spring then keeps the nib down across
any dips. See [setting the pen height](1stPlot.md#3-fit-the-pen-and-set-its-height).

Also check the pen is tight in the holder and the paper is flat and well secured.

## The plot started in the wrong place

The origin was not where you thought. Home the machine, set your zero again if the job
needs one, and check that your G-code was exported with an absolute origin.

## The pen crashes into the bed

Stop and cut power. Most often Z zero is set too low, or was set against a different
sheet — reset it with the nib on the paper you are actually using. If the machine
behaves as though it has the wrong toolhead, check its
[configuration](YAMLConfigurationSettings.md).

## Uploads take forever

Large plots are big files and the transfer is slow. Let it finish rather than
restarting it.

## Still stuck?

Ask on [Discord](https://discord.gg/fEXrmUm5nR). Include your toolhead type, what you
were doing, and anything the serial console printed.
