# Your first plot

This walks you through plotting one of the files already on the SD card. Do this
before making your own artwork — it proves the machine works and teaches you the
setup routine.

Before you start, make sure you have [powered up and connected](1sttimeuse.md).

## 1. Fit the paper

Take the calibration plot off the bed, turn it over, and put it back under the corner
tabs blank side up.

Line the paper up square to the machine — its edges parallel to the X axis — and get
it as flat as you can. A ripple in the paper becomes a wobble in the drawing.

## 2. Fit the pen and set its height

1. Pick the bung that best fits your pen barrel.
2. Push the pen through the bung and fit the assembly into the holder.
3. Set the height so the nib sits roughly **5 mm above the paper** when the pen is up.

Use the 2 mm puck as a reference for the pen-down position.

!!! tip "Pen height is the fiddly bit"
    This is the setting that most affects how a plot looks, and it takes practice.
    Too high and lines break up; too low and the nib drags, the paper tears, or the
    pen skips. Expect to adjust it for each new pen.

Check that the solenoid moved to its upright position when the machine powered on.

## 3. Home the machine

Homing tells the terraPen where it physically is. How you do it depends on whether
your machine has homing switches fitted.

<!-- TODO: confirm which of these two paths applies to machines shipping now, and
     which is the default in the current FluidNC configs. The terrapen-z-stepper
     config has limit switches enabled; terrapen-solenoid-relay has them commented
     out. See the documentation requirements list. -->

!!! warning "Check which applies to your machine"
    These two routines are not interchangeable. If you are unsure which your terraPen
    uses, ask on [Discord](https://discord.gg/fEXrmUm5nR) before running a homing
    cycle.

### If your machine has homing switches

Clear the bed, then press **Home** in the interface (or send `$H` in the serial
console). The carriage moves until it finds its switches and sets its own origin.

### If your machine does not have homing switches

There is nothing for the machine to find, so you set the origin by hand:

1. Jog the carriage to the **front left corner** of your paper.
2. Press **ZeroXY**.

## 4. Check your position

Before plotting, confirm the readout shows **X0, Y0** and the pen is up (**Z1** on a
solenoid machine).

If the numbers are not zero, the plot will start in the wrong place — go back to
step 3.

## 5. Run the plot

1. Refresh the **SD Files** panel (F) to list what is on the card.
2. Check the paper is secure and the pen is tight in the holder.
3. Press the **play** icon on the file you want to plot.

After a short pause of about ten seconds, the terraPen starts drawing.

!!! success "That's it"
    The artwork lives on the terraPen's SD card, so nothing needs to stay connected.
    You can close the browser, or unplug your laptop, and the plot carries on.

## Next steps

- [Make your own artwork with terraForge](terraForge.md)
- [Positioning work on the bed](plotting.md)
- Something went wrong? — [Troubleshooting](troubleshooting.md)
