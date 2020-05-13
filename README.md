# Linear Power Board
A board to take the input of two 15v SMPS AC-DC PSUs and output a precise, regulated +/-12v DC.

Using two 15v single-supply SMPSs*, the board combines the negative output of one supply with the positive output of the other supply, forming a reference ground.  The remaining positive output provides +15v to the board's negative rail and the remaining negative output provides -15v to the board's negative rail.
The positive and negative rails are then filtered before being regulated by a LM350 on the positive rail and an LM337 on the negative rail.  The two regulators can be adjusted using a trimmer to achieve exactly +/-12v DC at (depending on the heatsink and supply chosen) up to 2A** on the positive rail and 1.5A on the negative.

The boards use blade/faston terminals to distribute power to the busboards.

* Such as the Mean Well RS-35-15, RS-50-15 or the smaller LRS-35-15 / LRS-50-15 (or similarly specced)
** Theoretically it could provide 3A, but you would need a very large heatsink with active cooling.
Project is CC BY-NC-SA 4.0
