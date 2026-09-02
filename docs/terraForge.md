# Making artwork with terraForge

**terraForge is the recommended way to get your artwork onto the terraPen.** It is our
own desktop application, built for this machine, and it replaces most of the older
multi-step workflows described on the following pages.

- Download it from the [terraForge releases page](https://github.com/theworkisthework/terraForge/releases)
- Read the [full terraForge user guide](https://github.com/theworkisthework/terraForge/blob/main/docs/terraForge-user-guide.md)

## Why use it

With terraForge you can do the whole job in one place:

- Import **SVG** and **PDF** artwork, or open existing **G-code**
- Position, scale and rotate your work on an on-screen representation of the bed
- Generate G-code, with path optimisation to cut down wasted pen travel
- Preview the toolpath before you commit paper to it
- Connect over **Wi-Fi or USB**, upload straight to the SD card, and run the job
- Jog the machine, home it, and clear alarms without leaving the app

Previously this meant exporting from Inkscape or Lightburn, converting to G-code,
then uploading through the web interface by hand. terraForge does all of it.

## The basic workflow

1. **Set up your machine profile** — tell terraForge your bed size and how to reach
   your terraPen (Wi-Fi or USB).
2. **Connect** to the machine.
3. **Import** your SVG or PDF.
4. **Position** it on the bed and scale it to suit your paper.
5. **Generate G-code**, checking the previewed toolpath.
6. **Upload and plot** — send it to the SD card and press play.

The [user guide](https://github.com/theworkisthework/terraForge/blob/main/docs/terraForge-user-guide.md)
covers each step in detail, with screenshots.

!!! note "You still need to set up the machine itself"
    terraForge handles the artwork and the job. Fitting paper, setting pen height and
    homing are still done at the machine — see [Your first plot](1stPlot.md).

## Other tools

terraForge is the easiest route, but the terraPen plots standard G-code, so anything
that produces it will work. See [Uploading files](uploadingFiles.md) for the
alternatives, including [Lightburn](LightburnProfilesAndSettings.md).
