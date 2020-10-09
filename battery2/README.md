# battery2

Show the current status of your battery.

![](images/full.png)

![](images/charging.png)

![](images/unplugged.png)

![](images/unknown.png)

![](images/nobattery.png)

# Dependencies

fonts-font-awesome, acpi, python3

# Installation

To use with i3blocks, copy the blocklet configuration in the given `i3blocks.conf` into your i3blocks configuration file, the recommended config is

```INI
[battery2]
command=$SCRIPT_DIR/battery2
markup=pango
interval=30
```

Optionally notification command can be executed when battery level dropped below threshold:

```INI
[battery2]
LOW_NOTIFY=notify-send --icon=battery -u critical Battery "Too low battery!"
LOW_TRIGGER=10
```
