# PINN for fracture of material in Multiphysics Environment

### Problem Statement
- Predicting oxide concentration in the crack region part of the turbine blades is essential to find the load bearing capacity.
- Predicting fracture in such structure accounts for material heterogeneity and geometric complexity.
- This task is often challenging in terms of analyzing computationally and experimentally.

### Solution
- Physics Informed Neural Networks are used to solve the above problem.
- PINN (Physics informed neural networks) are neural networks modeled and trained to solve supervised learning tasks while considering governing laws of physics described by PDEs.

### Methodology
- Defining and importing required libraries for the underlying functions.
- Defining the range of spatial, temporal and combined domain.
- Applying initial and boundary conditions on the domain.
- Defining the governing PDEs on the domain.
- Defining the PDE module and supplying number of points.
- Creating a Neural Network and compiling the model.
- Training the model
- Validation using analytical and FEM solutions.

### Results
#### 1D Problems
##### 1D Diffusion with Neumann conditions
- On a bar, flux is applied on the left boundary with Neumann conditions
###### Result :
![1DDiffusionWithNeumannConditions](/neumann1d.gif "1D Diffusion with Neumann Conditions")

##### 1D Diffusion with Dirichlet conditions
- On a bar, flux is applied on the left boundary with Dirichlet conditions
###### Result :
![1DDiffusionWithDirichletConditions](/dirichlet1d.gif "1D Diffusion with Dirichlet Conditions")

##### 1D Diffusion with Robin conditions
- On a bar, flux is applied on the both the boundary with Neumann condtions
###### Result :
![1DDiffusionWithRobinConditions](/robin1d.gif "1D Diffusion with Robin Conditions")

#### 2D Problems
##### 2D Diffusion with Neumann conditions
- On a plate, flux is applied on the left boundary with Neumann conditions
###### Result :
<p float="left">
  <img src="/neumann2dpinn.gif" width="32%" />
  <img src="/neumann2danalytical.gif" width="32%" /> 
  <img src="/neumann2derror.gif" width="32%" />
</p>

##### 2D Diffusion with Dirichlet conditions
- On a plate, flux is applied on the left boundary with Neumann conditions
###### Result :
<p float="left">
  <img src="/dirichlet2dpinn.gif" width="32%" />
  <img src="/dirichlet2danalytical.gif" width="32%" /> 
  <img src="/dirichlet2derror.gif" width="32%" />
</p>

##### 2D Diffusion with Neumann conditions on partial boundary
- On a plate, flux is applied on bottom one-fourth of the left boundary with Neumann conditions
###### Result :
![2DDiffusionWithNeumannConditionsPartialBoundary](/neumann2dpartialboundary.gif "1D Diffusion with Robin Conditions")
