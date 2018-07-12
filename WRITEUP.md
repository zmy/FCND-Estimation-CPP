# Step 1: Sensor Noise
By calculating standard deviations from the log files, I find that GPS X data follow `N(0, 0.7)` and accelerometer X data follow `N(0, 0.5)`.
Thus I set `MeasuredStdDev_GPSPosXY = 0.7` and `MeasuredStdDev_AccelXY = 0.5`. Following is the simulation result:
<p align="center">
<img src="images/s1.png" width="500"/>
</p>

# Step 2: Attitude Estimation
By converting roll, pitch and yaw into quaternion and integrate body rate into the quaternion and then convert back, the nonlinear complementary filter is implemented as described in the document. Simulation result:
<p align="center">
<img src="images/s2.gif" width="500"/>
</p>
