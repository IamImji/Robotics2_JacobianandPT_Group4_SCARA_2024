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

<div align="center">

| *Jacobian Matrix Computaion*     |
|-----------------------       |
| [Jacobian-Matrix-Solutions.pdf](https://github.com/IamImji/Robotics2_JacobianandPT_Group4_SCARA_2024/files/15296741/Jacobian-Matrix-Solutions.pdf) |

</div>

## IV. Differential of SCARA Mechanical Manipulator description and computation.

## V. Path and Trajectory Planning of SCARA Mechanical Manipulator description and program.
## VI. References
* https://byjus.com/maths/jacobian/
* 
## VII. Members
* ###  Cullos, Kristina Crisandra M.
* ###  Francisco, Jestine Anne A. 
* ###  Garcia, Mark Jeffereson R.
* ###  Mirabel, Jan Andrei A.
* ###  Rayos, Christine Mae C.

