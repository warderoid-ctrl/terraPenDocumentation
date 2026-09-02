# YAML configuration settings

The terraPen runs [FluidNC](https://github.com/bdring/FluidNC). FluidNC is configured
by a `.yaml` file describing the machine — its motors, its toolhead, its limits and
its homing behaviour.

**Your terraPen arrives already configured**, with every supported YAML file loaded
and the correct one selected for your toolhead. You do not need to touch this to
plot.

## When you might change it

- You have swapped toolheads — each toolhead needs its matching YAML file.
- You want to adjust settings such as **acceleration** or **feedrate**.

Configuration files live in our
[fluidnc-config-files repository](https://github.com/theworkisthework/fluidnc-config-files).

## Selecting a configuration

The active file is set by the **Config/Filename** field in the controller settings:

![The Config/Filename setting](img/Settings Config.png)

Set it to the YAML file matching your toolhead, then restart the controller.

!!! warning "Match the file to your hardware"
    Loading a configuration for the wrong toolhead can drive the pen into the bed or
    make homing move the wrong way. If you are unsure which file is right for your
    machine, ask on [Discord](https://discord.gg/fEXrmUm5nR) before changing it.
