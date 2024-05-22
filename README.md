#  <p align="center">**Robotics 2: Jacobian Matrix and Path and Trajectory of a**</p>
# <p align="center">$${\color{red}**SCARA**}‎~~{\color{red}**Manipulator**}$$</p>

## I. Abstract of the Project
<div align="justify">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The paper explains the key methods for calculating the Jacobian matrix and designing paths and trajectories for a Selective Compliance Assembly Robot Arm (SCARA) manipulator. The Jacobian matrix is a fundamental concept in robotics that connects joint velocities to end-effector velocities in Cartesian space and provides information on the manipulator's kinematic features. Path and trajectory planning are essential for creating efficient and precise motion sequences that ensure smooth and collision-free movements. By investigating these techniques, this research hopes to improve our understanding and implementation of SCARA robots in industrial automation applications.</div>

## II. Introduction of the Project
***<div align="justify">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Selective Compliance Assembly Robot Arm (SCARA) Manipulators*** are commonly utilized in industrial automation due to their high efficiency and precision in activities including assembly, packing, and material handling. The SCARA robot's unique design, defined by horizontal motion and rotating joints, provides high vertical rigidity while maintaining horizontal compliance, making it excellent for applications requiring precise planar movements. Determining the Jacobian matrix and creating routes and trajectories are two essential steps in comprehending and utilizing the capabilities of a SCARA manipulator. An essential tool in robotics, the Jacobian matrix establishes a connection between the end-effector's velocity in Cartesian space and the joint velocities of the robot. We may learn more about the manipulator's kinematic behavior, including its singularities, manipulability, and force transmission properties, by examining the Jacobian.</div>

<div align="justify">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;On the other hand, path and trajectory planning entails creating the SCARA manipulator's motion sequence to accomplish desired tasks precisely and efficiently. This entails specifying the trajectory, or the time-based profile of motion along the path, and the path, or the geometric locus of points the end-effector will follow. Efficient planning guarantees seamless, collision-free motions, optimizing for parameters like velocity, precision, and energy usage. In this project, we will look at the approaches for calculating a SCARA manipulator's Jacobian matrix, as well as path and trajectory planning procedures. By combining these ideas, engineers and researchers can improve the performance and applicability of SCARA robots in a variety of industrial applications.</div>

## III. Jacobian Matrix of SCARA Mechanical Manipulator description and computation.

<div align="justify">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The term Jacobian often represents both the jacobian matrix and determinants, which is defined for the finite number of function with the same number of variables. Here, each row consists of the first partial derivative of the same function, with respect to the variables. The jacobian matrix can be of any form. It may be a square matrix (number of rows and columns are equal) or the rectangular matrix(the number of rows and columns are not equal).</div>

\
<div align="justify">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The Jacobian matrix is a fundamental notion in mathematics, particularly multivariable calculus. Its purpose is to depict the rate at which one set of variables changes in relation to another. In essence, if you have a function that maps from one vector space to another (like a multivariable function), the Jacobian matrix tells you how each output variable changes concerning each input variable.</div>

\
The concept of the Jacobian Matrix was first introduced by the mathematician ***Carl Gustav Jacob Jacobi*** in the 19th century.


<div align="center">
   
| *Jacobian Matrix*     |
|-----------------------       |
|![Screenshot 2024-05-13 222748](https://github.com/IamImji/Robotics2_JacobianandPT_Group4_SCARA_2024/assets/158303837/2555d036-1b17-4e08-81a8-01408716405a) |

</div>

> [!NOTE]
> Rows = no. of rows in End Effector Velocity Vector (always 6).
\
> Columns = no. of rows in DH Parametric Table.

**Methods of Obtaining Jacobian Matrix**
1. Partial Derivative Method
2. Propagation Method
3. Linear Algebra Method

<div align="center">
   
| *Linear Algebra Method*     |
|-----------------------       |
|![Screenshot 2024-05-13 225156](https://github.com/IamImji/Robotics2_JacobianandPT_Group4_SCARA_2024/assets/158303837/597b4d54-78e9-48bf-8ef5-b66c1aed4135) |


</div>

> [!NOTE]
> R = Rotation Matrix (follow the superscripts and subscripts)
\
> d = Position Vectors (follow the superscripts and subscripts)
\
> i = which column/joint you are solving at J
\
> n = no. of columns/joints of J

<div align="center">
   
| *Linear Algebra Method*     |
|-----------------------       |
| ![Screenshot 2024-05-13 225544](https://github.com/IamImji/Robotics2_JacobianandPT_Group4_SCARA_2024/assets/158303837/48e586cd-faf5-44e7-9d35-c8b9ef89a585) |

</div>

\
<div align="center">
   
|      *Jacobian Matrix Solutions*   | |
| ----------------------- |  ----------------------- |       
| ![Screenshot 2024-05-13 235158](https://github.com/IamImji/Robotics2_JacobianandPT_Group4_SCARA_2024/assets/158303837/cd21b2b8-470a-4ad1-b664-e375e110f25a)| ![Screenshot 2024-05-13 235230](https://github.com/IamImji/Robotics2_JacobianandPT_Group4_SCARA_2024/assets/158303837/81e1c96a-61ce-4f2b-b82b-2cf34b0de52d) 

![Screenshot 2024-05-13 235259](https://github.com/IamImji/Robotics2_JacobianandPT_Group4_SCARA_2024/assets/158303837/fd3bc477-d3ea-48be-96f8-ad534c3ef53c)

</div>

## IV. Differential Equation of SCARA Mechanical Manipulator description and computation.

<div align="center">
   
| *Differential Equation*     |
|-----------------------       |
| ![Screenshot 2024-05-18 123033](https://github.com/IamImji/Robotics2_JacobianandPT_Group4_SCARA_2024/assets/158303837/57267682-de04-46f3-aed9-fe41be9cd636) |

</div>

<div align="center">Here is the computation of Differential Equation of a SCARA Manipulator</div>

## V. Singularity of SCARA Mechanical Manipulator description and computation.


<div align="center">
   
| *Singularity*     |
|-----------------------       |
| ![Screenshot 2024-05-21 153149](https://github.com/IamImji/Robotics2_JacobianandPT_Group4_SCARA_2024/assets/158303837/d667a78d-8ce6-4c50-ae06-f093898c7c2d) |

</div>

## VI. Path and Trajectory Planning of SCARA Mechanical Manipulator description and program.

Path and trajectory planning are essential concepts in robotics and control systems.

***<div align="justify">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Path Planning*** entails determining a feasible path from a starting point to a destination while avoiding impediments. This task is critical for autonomous robots or vehicles to travel in complex situations safely and effectively. Path planning algorithms provide a set of connected waypoints or configurations that the robot can use to get to its destination.</div>

***<div align="justify">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Trajectory planning***, on the other hand, is concerned with creating smooth, possible trajectories for a robot to follow as it travels. These trajectories take into account robot dynamics, velocity profiles, and limitations such maximum speed and acceleration. The goal is to ensure that the robot moves smoothly and precisely from one location to another while taking into consideration its physical constraints and the dynamics of its surroundings.</div>

<div align="justify">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Robots require both route planning and trajectory planning as essential parts of their motion planning systems in order to navigate through a variety of real-world situations safely and successfully, avoiding collisions and maximizing movement efficiency. These ideas are used in mobile robots, industrial automation, and autonomous vehicles, among various other fields.</div>

\

<div align="center">
   
|      *Path and  Trajectory Pick and Place*   |   *Path and Trajectory Welding*        |
| ----------------------- |  ----------------------- |       
|  ![PandP](https://github.com/IamImji/Robotics2_JacobianandPT_Group4_SCARA_2024/assets/158303837/a63c4e8c-ec43-4f0d-839f-1f41c2e9ecdb) | ![welding](https://github.com/IamImji/Robotics2_JacobianandPT_Group4_SCARA_2024/assets/158303837/3c114d8d-2a4f-4c50-aa0e-76b0429fd439) |

</div>

## VII. References
* Admin. (2019, December 9). Jacobian Matrix and Determinant (Definition and Formula). BYJUS. https://byjus.com/maths/jacobian/

## VIII. Video Presentation
* Task 1
* Task 2
* Task 3
* Task 4 - https://youtu.be/5zxw8IW67yU?si=oYBMBsoTleLAnyBJ
* Task 5 - https://youtu.be/baRaOgWt2XM?si=kgcU3lggINRWqCAx
  
## VII. Members
* ###  Cullos, Kristina Crisandra M.
* ###  Francisco, Jestine Anne A. 
* ###  Garcia, Mark Jeffereson R.
* ###  Mirabel, Jan Andrei A.
* ###  Rayos, Christine Mae C.

