# Quench-Random-Spin

## Contents
This repository contains codes for plotting figures in the main text and the supplementary material, in the paper *Emergent Universal Quench Dynamics in Randomly Interacting Spin Models*.

- Packages

  - **Figure1**: Codes for Plotting Fig. 1b,c, which denotes the crystal structure; and Codes for Fig. 1d,e, which calculates the distribution of coupling strength $J_{ij}$, based on the crystal structure.
  
  - **Figure2**: Fitting codes for Fig. 2a-c, including the errorbar analysis; and plotting codes of Fig. 2.
  
  - **Figure4**: Plotting codes of Fig. 4.
    
  - **FigureS1**: Plotting codes of Fig. S1.
 
  - **FigureS3**: Plotting codes of Fig. S3.
 
  - **FigureS4**: Plotting codes of Fig. S4.
 
  - **FigureS5**: Plotting codes of Fig. S5.
   
## Dependence

- Mathematica 12.1 (or above)
  - Crystallica, https://library.wolfram.com/infocenter/MathSource/9372/

- Matlab R2022b (or above)
  - Curve Fitting Toolbox

## Running the program

- **Figure1**
    - Run `Crystal.nb` to plot the crystal and molecular structure.
    - Run `Jij_Distribution.mlx` to calculate and display the distribution of coupling strength $J_{ij}$, based on the crystal structure. You can change the parameter "rand_times", which is the number of random orientations for a powder sample.

- **Figure2**
    - Run `Process_quench_x.mlx`, `Process_quench_y.mlx`, `Process_quench_z.mlx` to fit the curves in Fig. 2a, Fig. 2b, Fig. 2c, respectively, getting the best fitting results of $\Lambda$ and $\Gamma$, and their errorbars estimated using the contour methods. Afterwards, the fitting results are fed into `PlotCode_x`, `PlotCode_y`, `PlotCode_z`, respectively.
    - Run `PlotCode_x`, `PlotCode_y`, `PlotCode_z` to plot Fig. 2a,d,g, Fig. 2b,e,h, Fig. 2c,f,i, respectively.

- **Figure4**
    - Run `Process.mlx` to plot Fig. 4.

- **FigureS1**
    - Run `Process.mlx` to plot Fig. S1.
      
- **FigureS3**
    - Run `Process.mlx` to plot Fig. S3.
    - 
- **FigureS4**
    - Run `Process_ab.mlx` to plot Fig. S4ab.
    - Run `Process_cdef.mlx` to plot Fig. S4cdef.
      
- **FigureS5**
    - Run `Process.mlx` to plot Fig. S5.

 
## Contact

Email: lyuchen@mail.ustc.edu.cn or mrtuhao232@gmail.com
