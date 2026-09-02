# Moving the pen carriage

There are two ways to move the carriage.

## By hand

**Only with the machine powered off.** Push the carriage gently. Never force it
against the ends of its travel.

## With the jog wheel

Use the jog wheel in the **Controls** panel (B). Click a segment to move the carriage
in that direction. The distance depends on which ring you click:

| Ring | Distance per click |
|---|---|
| Outer | 100 mm |
| Second | 10 mm |
| Third | 1 mm |
| Inner | 0.1 mm |

Start with a large step to get close, then work inwards for fine positioning.

## Raising and lowering the pen

Use the **Pen Up** and **Pen Down** macros rather than jogging the Z axis directly.

!!! warning "Z behaviour depends on your toolhead"
    What the Z axis does varies between toolheads. On a solenoid machine, **Z0 is pen
    down and Z1 is pen up**. On a servo or Z-stepper toolhead the range is different.
    Jogging Z by hand can drive the pen into the bed, so use the macros unless you know
    your machine's configuration.
