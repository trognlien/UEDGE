# UEDGE
2D fluid simulation of plasma and neutrals in magnetic fusion devices
# Brief description 
UEDGE is an interactive suite of physics packages using the Python or BASIS scripting systems. 
The original (circa 2007) Python version was further developed under the FACETS SciDAC project 
[Cary 2008, McCourt 2012]. The plasma is described by time-dependent 2D plasma fluid equations 
that include equations for density, velocity, ion temperature, electron temperature, electrostatic 
potential, and gas density in the edge region of a magnetic fusion energy confinement device. slab, 
cylindrical, and toroidal geometries are allowed, and closed and open magnetic field-line regions 
are included. Classical transport is assumed along magnetic field lines, and anomalous transport 
is assumed across field lines.  Multi-charge state impurities can be included with the corresponding 
line-radiation energy loss. 

# Method of solution
A fully implicit numerical algorithm is used that allows both Newton-like iterations to steady state 
and time-dependent solutions with large time-steps.  A preconditioning matrix is obtained by approximate 
(ILUT) inversion of a numerical finite-difference Jacobian, which is then used in a Newton-Krylov 
solution algorithm.

# Authors contributing to V7 release
T.D. Rognlien, I. Joseph, W.H. Meyer, M.E. Rensink, and M.V. Umansky, LLNL

# Acknowledgements to previous contributors
P.N. Brown, R.H. Cohen, D.P. Grote, A.C. Hindmarsh, L.L. LoDestro, J.L. Milovich, 
A. Pankin, G.D. Porter, and G.R. Smith, all presently or formerly at LLNL; M. McCourt, 
L.C. McInnes, and H. Zhang, ANL; J.R. Cary, A.H. Hakim, S.E. Kruger, and A. Pankin, Tech-X; 
D.A. Knoll, INEEL; D.P. Stotler, PPPL; B.J. Braams, retired, IAEA; A.Yu. Pigarov and 
R. Smirnov, UCSD; J.D. Elder, U. Toronto; M. Groth, Aalto Univ.; and R.B. Campbell, Sandia.
