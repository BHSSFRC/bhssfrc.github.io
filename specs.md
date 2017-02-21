# specs

so here's some technical specs for future reference.

## UnitTypes
* Any method that takes a UnitTypes constant as a parameter **must** respect that type as follows:
  * No two UnitTypes should return equal results.
  * In distance measurements, all measurements **must** be `double`s. __No `float`s allowed.__
  * For conversions, one inch is **exactly** equal to 2.540 centimeters, 25.400 millimeters, and 1/12 of a foot.

## DriveDirections
* Only special thing here is that you don't necessarily need to respect `DriveDirections.UP` and `DriveDirections.DOWN` (these only pertain to climbing subsystems.)

## Fields
* Subsystems **must**:
  * Keep all fields which represent motor controllers, encoders, and other hardware private.
  * not have setters and getters for hardware fields
  * allow other classes to access relevant methods of the hardware via public methods.
* Commands **must**:
  * NEVER, EVER, EVER have static fields. **EVER.**

A field may be static if and only if you are confident you know what you are doing, is ***not*** in a command, or if it's in the `Robot` class.
