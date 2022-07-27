# Robotic Arm

## Design and Simulation

Designing the robot arm, Cinema4D was used and Null Function was also used for simulation purposes.
In each joint connecting the different parts, bearing was install to minimize friction and allow smoother motions.

![robot arm 1](https://user-images.githubusercontent.com/109004035/181239615-804b4b48-1ad0-4c9e-92f9-39436f083fd9.jpg)
![robot arm 2](https://user-images.githubusercontent.com/109004035/181239623-d8762b79-4396-4f19-8cb0-6b993ed896bd.jpg)


### Degrees of freedom

Degrees of freedom are the maximum number of logically independent, or potentially different, values in the sample of data. When discussing various types of statistical hypothesis testing, degrees of freedom are frequently brought up.

### System Discussion

This is a design of a 3 DOF Robotic arm. In this design, the base is only able to rotate on the XY_ plane.
In the design, there are only 2 links, and each joint is able to move upward and downwards, meaning if we were to neglect or ignore the base movement, the system is to be considered in 2D, or one plane of movement!
this can simplify understanding how the robotic arms function, and how its possible to study them and make the proper calculations.

### Forward Kinematics

Forward kinematics is the technique of determining the end effector's location and velocity from known joint angles and angular velocities. The objective is to determine the Cartesian coordinates of the wrist and fist, for instance, if the shoulder and elbow joint angles for the arm in the sagittal plane are supplied.

### System Analysis
To determine how to reach an end point, multiple functions with multiple variables are to be used depending on the number of joints and the DOF of our system! and it's very common to go through this process using matrices. However! for this specific system, it's very easy to determine how to reach an end point, due to the fact the it's a 3 DOF system with only 2 joints to consider**( ignoring the base rotation until fixing the 2 components of the joints!)**

To calculate an end point of the 2 Joints in 2D or in one plane, we can use 2 equations with 2 variables! 

![forward kinematics](https://user-images.githubusercontent.com/109004035/181238530-afee6ff9-9f99-437f-b7eb-2d1ad177cdad.jpg)


it's easy to determine the X and Y components of the end point considering it a vector !
after that, we try to reach to these values using Trigonometric concepts and considering each link length.

After fixing the X and Y components of the end point, then we can take the base rotation into consideration fixing the last components of our end point.

If we were to introduce one more joint, for example, then we are basically introducing one more equation and variable to the calculations, and so on!


