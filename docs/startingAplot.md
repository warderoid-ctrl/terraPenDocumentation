# Starting, pausing and cancelling a plot

## Starting

1. Find your `.g` file in the **SD Files** panel (F).
2. Press the **play** icon on that row.
3. The plot begins after a pause of about ten seconds.

!!! warning "Zero the machine first"
    Always set your origin before plotting — see
    [Your first plot](1stPlot.md#3-home-the-machine). Starting a job from the wrong
    position is the most common way to spoil a sheet.

## While it runs

The **Job progress** panel (E) shows a progress bar with **Pause** and **Cancel**
buttons.

Pausing stops the carriage where it is. The pen lifts, so it will not bleed into the
paper while you wait.

## After cancelling

Cancelling a plot puts the machine into an **alarm** state. This is normal and is the
firmware protecting itself, because it no longer trusts its position.

To clear it, click the **Alarm** button at the left of the message, or send `$X` in
the serial console.

!!! note "Nothing works until the alarm is cleared"
    While the alarm is active you cannot jog the machine or start another plot.

After clearing an alarm, re-establish your origin before plotting again.
