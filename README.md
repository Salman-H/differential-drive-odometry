# differential-drive-odometry
Differential-drive robot odometry with IR sensors and wheel encoders using simiam. Implemented as part of a Georgia Tech Mobile Robotics course project.

Simiam is a MATLAB-based educational bridge between theory and practice in robotics created at Georgia Tech GRITS Lab.

1. Robot goes straight if theta = 0:
<img src="https://github.com/Salman-H/differential-drive-odometry/blob/master/figures/Inked1_bot_theta_0_LI.jpg" alt="bot theta 0" width="200">

2. Without odometry implemented, robot will rotate around its initial coordinate for a non-zero theta:
<img src="https://github.com/Salman-H/differential-drive-odometry/blob/master/figures/Inked2_bot_theta_45_no_odometry_LI.jpg" alt="bot no odometry" width="200">