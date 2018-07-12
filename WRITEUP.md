# Step 1: Sensor Noise
By calculating standard deviations from the log files, we find that GPS X data follow `N(0, 0.7)` and accelerometer X data follow `N(0, 0.5)`.
Thus we set `MeasuredStdDev_GPSPosXY = 0.7` and `MeasuredStdDev_AccelXY = 0.5`. Following is the simulation result:
<p align="center">
<img src="images/s1.png" width="500"/>
</p>
