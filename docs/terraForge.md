# terraForge

**terraForge is how we recommend you drive the terraPen.** It is our own desktop
application, built for this machine, and it replaces the older multi-step workflows of
exporting, converting and uploading by hand.

- [Download the latest release](https://github.com/theworkisthework/terraForge/releases)
- [Full terraForge user guide](https://github.com/theworkisthework/terraForge/blob/main/docs/terraForge-user-guide.md)

!!! note "Take the latest release candidate"
    terraForge is under active development, so the newest build is normally an **RC**
    release. That is the one to install — it is where the current work lands.

## What it does

- Import **SVG** and **PDF** artwork, or open existing **G-code**
- Position, scale and rotate work on an on-screen representation of the bed
- Generate G-code with path optimisation, so the pen wastes less time travelling
- Preview the toolpath before committing paper to it
- Connect over **Wi-Fi or USB**, upload to the SD card, and run the job
- Jog, home, set Z zero, raise and lower the pen, and clear alarms

The stepper toolhead is the **default** in terraForge, so a new machine should work
without any configuration changes.

## The basic workflow

1. **Set up your machine profile** — bed size, and how to reach the plotter.
2. **Connect** over Wi-Fi or USB.
3. **Import** your SVG or PDF.
4. **Position** it on the bed and scale it to your paper.
5. **Generate G-code**, checking the previewed toolpath.
6. **Upload and plot.**

The [user guide](https://github.com/theworkisthework/terraForge/blob/main/docs/terraForge-user-guide.md)
covers every step in detail, with screenshots.

## Wi-Fi or USB

Both work. If you want to use USB rather than Wi-Fi, select it in terraForge's
**machine settings** — see [Connect via USB-C](ConnectTethered.md).

## Feedback

terraForge is developed in the open, and questions, suggestions and bug reports are
genuinely wanted. Bring them to
[our Discord](https://discord.gg/fEXrmUm5nR).

!!! note "You still set the machine up by hand"
    terraForge handles artwork and jobs. Fitting paper and setting pen height still
    happen at the machine — see [Your first plot](1stPlot.md).
