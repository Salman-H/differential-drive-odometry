# differential-drive-odometry
Differential-drive robot odometry with IR sensors and wheel encoders using simiam. Implemented as part of a Georgia Tech Mobile Robotics course project.

Simiam is a MATLAB-based educational bridge between theory and practice in robotics created at Georgia Tech GRITS Lab.

<h4>1. Robot goes straight if theta = 0:</h4>
<img src="https://github.com/Salman-H/differential-drive-odometry/blob/master/figures/Inked1_bot_theta_0_LI.jpg" alt="" width="500">

<h4>2. Without odometry implemented, robot will rotate around its initial coordinate for a non-zero theta:</h4>
<img src="https://github.com/Salman-H/differential-drive-odometry/blob/master/figures/Inked2_bot_theta_45_no_odometry_LI.jpg" alt="" width="500">

<h4>3. A P-regulator uses the theta calculated from odometry to steer the robot to a specified heading of 45 degrees:</h4>
<img src="https://github.com/Salman-H/differential-drive-odometry/blob/master/figures/Inked2_bot_theta_45_with_odometry_LI.jpg" alt="" width="500">

The actual robot position can be compared to the odometry-estimated position to test odometry implementation.

initial pose:
<br />
<img src="https://github.com/Salman-H/differential-drive-odometry/blob/master/figures/3_a_bot_final_pose.PNG" alt="" width="600">

final pose:
<br />
<img src="https://github.com/Salman-H/differential-drive-odometry/blob/master/figures/3_b_bot_final_pose.PNG" alt="" width="600">

<h4>4. The five on-board IR range sensors independantly detect obstacles:</h4>
<img src="https://github.com/Salman-H/differential-drive-odometry/blob/master/figures/Inked4_bot_ir_skirt_LI.jpg" alt="" width="500">

The IR sensors have a range of upto 30 cm or 0.3 m. Skirts from sensors 1, 2 and 5 are not yet in range of the wall corner and, therefore,
read approximately 0.3 m as no obstacle is detected in their skirts. Sensors 3 are 4 are closer than 0.3 m to the corner and, therefore, 
read shorter distances.

<img src="https://github.com/Salman-H/differential-drive-odometry/blob/master/figures/Inked5_bot_ir_obstacle_LI.jpg" alt="" width="400">
