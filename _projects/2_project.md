---
layout: page
title: Python & C++ Fem
description: Linear Finite Element Method (FEM) for simulating hyperelastic cubes
img: /assets/img/imp.gif
importance: 2
category: work
related_publications: false

---
&#x1F4C2; [C++ code is available here!](https://github.com/Yuxing-Wang-THU/FEM)<br />

&#x1F4C2; [Python code is available here!](https://github.com/Yuxing-Wang-THU/PythonFem)<br />

<img src="/assets/img/Multiple_2D_Neohookean_implicit_False_bend_8.gif" div align=middle width = "49%" /><img src="/assets/img/Multiple_2D_Neohookean_implicit_False_fall_8.gif" div align=middle width = "49%" />

Linear Finite Element Method (FEM) for simulating hyperelastic cubes, all codes are based on pure Python or C++.

## Overview 

| Constitutive Models |  Time Integration | Multiple cubes  | 
| :------------- | :----------: | :----------: | 
| Linear Elasticity           |    Symplectic Euler   |  Yes  |
| St. Venant-Kirchhoff        |    Symplectic/Implict Euler   | Yes  |
| Corotated linear elasticity |    Symplectic Euler   |  Yes  |
| Neohookean elasticity       |    Symplectic/Implict Euler   |  Yes |

## Visual Results of a single Triangle
<p align="center">Symplectic Euler Methods</p>

<img src="/assets/img/single_2D_Linear_implicit_False.gif" div align=middle width = "49%" /><img src="/assets/img/single_2D_STVK_implicit_False.gif" div align=middle width = "49%" />

<img src="/assets/img/single_2D_Co-rotated_implicit_False.gif" div align=middle width = "49%" /><img src="/assets/img/single_2D_Neohookean_implicit_False.gif" div align=middle width = "49%" />

<p align="center">Implict Euler Methods</p>

<img src="/assets/img/single_2D_STVK_implicit_True.gif" div align=middle width = "49%" /><img src="/assets/img/single_2D_Neohookean_implicit_True.gif" div align=middle width = "49%" />


## Visual Results of Multiple Cubes
<p align="center"> Symplectic Euler Methods </p>

<p align="center"> Linear Elasticity </p>

<img src="/assets/img/Multiple_2D_Linear_implicit_False_bend_8.gif" div align=middle width = "49%" /><img src="/assets/img/Multiple_2D_Linear_implicit_False_fall_8.gif" div align=middle width = "49%" />

<p align="center"> St. Venant-Kirchhoff </p>

<img src="/assets/img/Multiple_2D_STVK_implicit_False_bend_8.gif" div align=middle width = "49%" /><img src="/assets/img/Multiple_2D_STVK_implicit_False_fall_8.gif" div align=middle width = "49%" />

<p align="center"> Corotated linear elasticity </p>

<img src="/assets/img/Multiple_2D_Co-rotated_implicit_False_bend_8.gif" div align=middle width = "49%" /><img src="/assets/img/Multiple_2D_Co-rotated_implicit_False_fall_8.gif" div align=middle width = "49%" />

<p align="center"> Neohookean elasticity </p>

<img src="/assets/img/Multiple_2D_Neohookean_implicit_False_bend_8.gif" div align=middle width = "49%" /><img src="/assets/img/Multiple_2D_Neohookean_implicit_False_fall_8.gif" div align=middle width = "49%" />

<p align="center"> Implict Euler Methods </p>

<p align="center"> St. Venant-Kirchhoff </p>

<img src="/assets/img/Multiple_2D_STVK_implicit_True_bend_8.gif" div align=middle width = "49%" /><img src="/assets/img/Multiple_2D_STVK_implicit_True_fall_8.gif" div align=middle width = "49%" />

<p align="center"> Neohookean elasticity </p>

<img src="/assets/img/Multiple_2D_Neohookean_implicit_True_bend_8_inv.gif" div align=middle width = "49%" /><img src="/assets/img/Multiple_2D_Neohookean_implicit_True_fall_8.gif" div align=middle width = "49%" />


## Reference
[FEM Simulation of 3D Deformable Solids: A practitioner's guide to theory, discretization and model reduction](http://viterbi-web.usc.edu/~jbarbic/femdefo/)