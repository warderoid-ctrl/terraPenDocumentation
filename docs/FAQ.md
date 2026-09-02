# Frequently asked questions

The terraPen is developed continuously, and its workflow differs from other plotters
on the market. These are the questions we hear most often.

For symptom-by-symptom help, see [Troubleshooting](troubleshooting.md).

## Does it need assembling?

A little. The stepper toolhead ships unattached — four screws with the supplied hex
key. See [Fitting the toolhead](assembly.md).

## Is there an on/off switch?

No. The terraPen powers on as soon as it has power. Switch it off at the wall, or use
a switched extension lead or smart plug.

## What software should I use?

[terraForge](terraForge.md) — our own application, built for this machine. The
terraPen also plots standard G-code, so other tools work; see
[Uploading files](uploadingFiles.md).

## How big can I plot?

A full A2 sheet — 594 × 420 mm.

## Do I need a computer connected while it plots?

No. Artwork is stored on the terraPen's SD card, so once a plot starts you can close
terraForge or take your laptop away.

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

## Why does it go into alarm after I cancel a plot?

Because the firmware no longer knows where the pen is. Clear the alarm, then home the
machine again.
