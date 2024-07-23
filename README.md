# Quench-Random-Spin

## Contents
This repository contains codes for plotting figures in the main text and the supplementary information, in the paper *Emergent Universal Quench Dynamics in Randomly Interacting Spin Models*.

- Packages

  - **Figure1**: Codes for Plotting Fig. 1b,c, which denotes the crystal structure; and Codes for Fig. 1d,e, which calculates the distribution of coupling strength $J_{ij}$, based on the crystal structure.
  
  - **Figure2**: Exp data for dynamics of the auto-correlation function. Fitting codes for Fig. 2a-c, including the error bar analysis; and plotting codes of Fig. 2. 
  
  - **Figure4**: Exp data for dynamics of the multiple quantum coherence. Plotting codes of Fig. 4.
    
  - **FigureS1**: Numerical Simulation on the effect of static field inhomogeneity on spin dynamics.
 
  - **FigureS2**: Exp data of free induction decays and calibration of the dipolar coupling strength J.
 
  - **FigureS3**: Exp data for time-scale comparision between the dipolar Hamiltonian and the Floquet Hamiltonian.
 
  - **FigureS5**: Exp data for verification of the dipolar-ordered state, and corresponding optimization of prethermalization parameters.
 
  - **FigureS6**: Exp data for verification of prethermalization for different Hamiltonian configurations.

  - **FigureS7**: Numerical and Exp data on how the MQC ratio I_2/I_0 relies on the average pulse interval tau, showing the occurrence of transient pulse effects. 
    
  - **FigureS8**: Exp data on the calibration results of the Hamiltonian parameters.
 
  - **FigureS9**: Numerical simulation of the residual Hamiltonian from higher-order Magnus terms.
 
  - **FigureS10**: Exp data for comparison of dynamics between the auto-correlation function and the zero and the double quantum coherences, revealing a doubling relationship among the oscillation frequencies.
   
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
    - Run `Plot.mlx` to plot Fig. 4.

- **FigureS1**
    - Run `Simu_evolution_with_inhomogeneity.mlx` to run the simulation.
      
- **FigureS2**
    - Run `Process.mlx` to plot Fig. S2.
      
- **FigureS3**
    - Run `Process2.mlx` to plot Fig. S3.
      
- **FigureS5**
    - Run `Process_ab.mlx` to plot Fig. S4ab.
    - Run `Process_cdef.mlx` to plot Fig. S4cdef.
      
- **FigureS6**
    - Run `Process.mlx` to plot Fig. S6.

- **FigureS7**
    - Run `Process_exp.mlx` to get the data in Supplementary Figure 7c; run `Simu_MQCratio_versus_tau.mlx` to get the numerical results in Supplementary Figure a,b, by setting values for      
      'FiniteWidthPulse=1; %FiniteWidthPulse--1, Ideal (delta) pulse--0'
      'FlipAngleError=0;'.
    - Run `Plot.mlx`.
      
- **FigureS8**
    - Run `Process.mlx` to plot Fig. S8.
            
- **FigureS9**
    - Run `NumericalCalculation.mlx` to calculate the data used for Fig.S6. The adjustable parameters are: "nqubit"--number of qubits; "ave"--number of disorder realizations; "tau_seq"--the set of average pulse interval "tau".
    - Acknowledgements: the two subfunctions below are downloaded from Matlab open resources:
      David Terr (2023). ClebschGordan.m (https://www.mathworks.com/matlabcentral/fileexchange/5276-clebschgordan-m), MATLAB Central File Exchange. Retrieved October 19, 2023.
      Kobi (2023). Wigner3j symbol (https://www.mathworks.com/matlabcentral/fileexchange/20619-wigner3j-symbol), MATLAB Central File Exchange. Retrieved October 19, 2023.
      
 - **FigureS10**
    - Run `Plot.mlx` to plot Fig. S10.

   
## Contact

Email: lyuchen@mail.ustc.edu.cn or mrtuhao232@gmail.com
