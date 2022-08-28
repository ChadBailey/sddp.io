# USB-C Technical Details

!> This page is **under construction**, expect frequent major updates and
corrections until this banner is removed.

## USB-C Power Delivery

> The Steam Deck requires USB-C PD of 45 watts

USB-C has improved upon the USB specification in many ways. Among them is the
ability to specify the _maximimum wattage that can be delivered_ known as USB-C
PD or Power Delivery.

Since the Steam Deck requires 45 watts of PD, if you use a 100watt PD charger it
will work and supply it the full power necessary. It will also not be any faster
at charging than a 45watt PD charger since the Steam Deck only supports 45watts.
The charger that comes with the Steam Deck is 45watts.

If on the other hand you use a 30watt PD power supply, it will still technically
work with the Steam Deck. As a consequence of not having full power, the Steam
Deck will either be charged slower if turned off, or will slowly discharge while
being used. USB-C connections or wires not supporting the USB-C PD spec will
likely not work to charge the Steam Deck at all.

## Some Details About Docking Stations

> The Steam Deck supports USB-C DP & MST, capable of connecting at least 3
> external monitors in addition to the built-in screen when using 1080p
> monitors. 4k monitors are also supported of course, but unsure of impact to
> streams.
>
> All extra monitors will show black in "gaming mode", but when switching to
> "desktop mode", the desktop is extended appropriately.

The term "dock" gets used too loosely to be a useful definition, so not all
docks are created equal.

Some docking stations, particularly "universal" ones, often have very slow USB
video cards in them. This causes lots of performance, usability, and stability
issues. The tradeoff though is it will work to extend the monitors of even
computers that do not support DP over USB-C or DP MST.

If you see a dock with any reference to "DisplayLink", I recommend avoiding it.

The recommended dock in the [accessories page](accessories.md) uses DisplayPort
over USB to deliver the output directly from your Steam Deck to your monitor.
From there, the Display Port signal is split to create a unique display for each
monitor plugged in using a technology called
[DisplayPort Multi-Stream Transport (DP MST)](https://www.tripplite.com/products/ulti-stream-transport-mst-hub-technology).

The SteamDeck supports DP _and_ MST over USB-C, but devices that do not support
DP over USB-C will not work at all. Devices that support DP over USB-C but do
not support MST (Older MacBooks) will only be able to show the same display
duplicated output to every monitor. This is a PC limitation, not a limitation
with the dock.

For these reasons, your laptop may also work flawlessly with this docking
station. Unfortunately though, it can be hard to tell when shopping for laptops
since this information (particularly DP MST) isn't often easy to find.

Most gaming laptops with discrete graphics cards and USB-C do support DP and
MST, and the video out from the USB-C port is usually wired to the discrete
graphics card (more powerful one).
