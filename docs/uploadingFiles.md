# Uploading files

The terraPen draws from **G-code** files — plain text instructions describing where to
move and when to raise and lower the pen.

!!! tip "The easy route"
    [terraForge](terraForge.md) generates G-code from your artwork and uploads it to
    the machine for you. Use it unless you have a reason not to — the rest of this
    page describes doing it by hand.

## Making G-code

Any tool that outputs G-code will work:

| Tool | Notes |
|---|---|
| [terraForge](terraForge.md) | **Recommended.** Built for the terraPen; SVG and PDF in, plot out. |
| [Lightburn](LightburnProfilesAndSettings.md) | Designed for laser cutters, but produces very well optimised G-code. Profiles provided. |
| Inkscape | Various G-code plugins available. |
| DrawingBotV3 | Converts images into plottable line work and outputs G-code. |
| vpype | Command line toolkit for plotter work. |
| Laserweb | Browser-based G-code generation. |
| Your own code | Generative work can output G-code directly. |

Save files with a `.g` extension.

## Uploading through the web interface

1. Go to the **SD Files** panel (F).
2. Click **Upload**.
3. Select your file or files and click **Open**.

A progress indicator appears while the files transfer.

!!! note "Large files take a while"
    Detailed plots can be several megabytes, and the upload is not fast. Let it finish
    before starting a job.

## Managing files on the card

- **Folders** — click the *add folder* icon to create one, then open it to upload
  inside. Worth doing once you have more than a handful of plots.
- **Deleting** — click the *trashcan* icon on a file's row.
- **Space** — total SD card usage is shown at the bottom of the panel.
