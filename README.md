# D2K Damaged Units Data

Compares D2K vehicle speed in damaged and not damaged states

The time measurements were done by playing recordings in VLC player, and measuring the seconds when an event happens. Thus we have some minimal precision error of one second.

Here are the columns that can be found in the data
1. **Unit Type**
2. **Speed:** The average vehicle moving speed. Measured for distances of 7-9 cells.
3. **Speed Tol:** The speed is computed by dividing the distance over the duration. As we can't measure the duration precisely, we give this column which is the estimated maximal error for speed
4. **Status:** Describes the state of the vehicle when measuring the speed. Can be one of ["Damaged", "Smoking", "Intact"]. The "Intact" means that the health is on 100%. When the health is below 50% it will be either "Smoking" (emitting smoke particles) or "Damaged" (not emitting smoke particles). Note that "Smoke Duration" can be positive for the status "Damaged". It means that the smoke was extinguished when we started measuring the speed.
5. **Smoke Duration:** The smoke effect duration in seconds. Has precision of ±1 sec.
6. **Health Color:** The color of the health bar of the unit
