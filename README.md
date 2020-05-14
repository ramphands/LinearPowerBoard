# Linear Power Board for Eurorack

![linear power board](/linearpowerboard.jpg)
A board to take the input of two 15v SMPS AC-DC PSUs and output a precise, regulated +/-12v DC to use in a Eurorack system.

Using two 15v single-supply SMPSs*, the board combines the negative output of one supply with the positive output of the other supply, forming a reference ground.  The remaining positive output provides +15v to the board's negative rail and the remaining negative output provides -15v to the board's negative rail.
The positive and negative rails are then filtered before being regulated by a LM350 on the positive rail and an LM337 on the negative rail.  The two regulators can be adjusted using a trimmer to achieve exactly +/-12v DC at (depending on the heatsink and supply chosen) up to 2A** on the positive rail and 1.5A on the negative.  This is roughly enough power for a 9U 104HP case.

The boards use blade/faston terminals to distribute power to the busboards.

There is no 5v regulator or rail provided due to its huge decline in usage.  If needed, please either use a busboard with a 5v regulator or a solution such as the Mutable Instruments Volts plug-in module.

* Common examples are the Mean Well RS-35-15, RS-50-15 or the smaller LRS-35-15 / LRS-50-15 (or similarly specced)
** Theoretically it could provide 3A, but you would need a very large heatsink with active cooling.

Project is CC BY-NC-SA 4.0
