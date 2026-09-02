# Frequently asked questions

The terraPen is developed continuously, and its workflow differs from other plotters
on the market. These are the questions we hear most often.

For symptom-by-symptom help, see [Troubleshooting](troubleshooting.md).

## Does it need assembling?

A little. The stepper toolhead ships unattached — four screws with the supplied hex
key. See [Fitting the toolhead](assembly.md).

## Where is the power switch?

At the **rear right** of the plotter. Plug the adaptor in, then switch it on there.

## What software should I use?

[terraForge](terraForge.md) — our own application, built for this machine. The
terraPen also plots standard G-code, so other tools work; see
[Uploading files](uploadingFiles.md).

## How big can I plot?

A full A2 sheet — 594 × 420 mm.

## Do I need a computer connected while it plots?

No. Artwork is stored on the terraPen's SD card, so once a plot starts you can close
terraForge or take your laptop away.

**But if you disconnect, do not reconnect until the plot has finished.** Reconnecting
part way through can stall the controller and end the plot. If you think you might
want to pause, stay connected from the start — see
[deciding whether you are staying](startingAplot.md#decide-whether-you-are-staying).

## Can I check on a plot from another room?

Only if you stayed connected. Reconnecting to a running plot risks ending it, so if
you have already walked away, leave it to finish.

## Can I use USB instead of Wi-Fi?

Yes. Select USB in terraForge's machine settings — file upload works over the cable
too. See [Connect via USB-C](ConnectTethered.md).

## Should I home the machine every time?

Yes. The terraPen has limit switches, so homing is the reliable way to establish
position. You can still set your own zero afterwards if a job needs to start
somewhere specific.

## How do I set the pen height?

Bring the nib to the paper, set Z zero, then jog up 5 mm. Aim to set zero
*fractionally into* the paper so the spring keeps the pen down over any dips in the
bed. See [Your first plot](1stPlot.md#3-fit-the-pen-and-set-its-height).

## What pens can I use?

Most pens fit. Pen height matters far more than pen brand.

## Why does it go into alarm when I abort a plot?

Because the firmware no longer knows where the pen is. Clear the alarm and home the
machine again — occasionally it needs a full power cycle first.

You can usually avoid it: **pause** rather than abort. Pausing stops the machine
safely and lets you resume. See
[pause first](startingAplot.md#stopping-a-plot-pause-first).

## Can I stop a plot part way and carry on later?

Yes — that is exactly what **Pause** is for. The pen lifts and the machine waits until
you resume.
