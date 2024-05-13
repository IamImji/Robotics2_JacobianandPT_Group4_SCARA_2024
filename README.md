# Robotics2_JacobianandPT_Group4_SCARA_2024

## I. Abstract of the Project
## II. Introduction of the Project

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
| ![Screenshot 2024-05-13 222748](https://github.com/IamImji/Robotics2_JacobianandPT_Group4_SCARA_2024/assets/158303837/93cc65cd-bfe4-4e56-aae9-40cc2b7e9e33) |

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

## IV. Differential of SCARA Mechanical Manipulator description and computation.

## V. Path and Trajectory Planning of SCARA Mechanical Manipulator description and program.

Path and trajectory planning are essential concepts in robotics and control systems.

***<div align="justify">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Path Planning*** entails determining a feasible path from a starting point to a destination while avoiding impediments. This task is critical for autonomous robots or vehicles to travel in complex situations safely and effectively. Path planning algorithms provide a set of connected waypoints or configurations that the robot can use to get to its destination.</div>

***<div align="justify">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Trajectory planning***, on the other hand, is concerned with creating smooth, possible trajectories for a robot to follow as it travels. These trajectories take into account robot dynamics, velocity profiles, and limitations such maximum speed and acceleration. The goal is to ensure that the robot moves smoothly and precisely from one location to another while taking into consideration its physical constraints and the dynamics of its surroundings.</div>

<div align="justify">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Robots require both route planning and trajectory planning as essential parts of their motion planning systems in order to navigate through a variety of real-world situations safely and successfully, avoiding collisions and maximizing movement efficiency. These ideas are used in mobile robots, industrial automation, and autonomous vehicles, among various other fields.</div>

## VI. References
* https://byjus.com/maths/jacobian/
* 
## VII. Members
* ###  Cullos, Kristina Crisandra M.
* ###  Francisco, Jestine Anne A. 
* ###  Garcia, Mark Jeffereson R.
* ###  Mirabel, Jan Andrei A.
* ###  Rayos, Christine Mae C.

