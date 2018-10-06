# UEDGE
2D time-dependent fluid simulation of plasma and neutrals in magnetic fusion devices.
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
solution algorithm. Over 95% of the coding is in Fortran with the remainder being C.

# Authors contributing to V7 release
T.D. Rognlien, I. Joseph, W.H. Meyer, M.E. Rensink, and M.V. Umansky, LLNL  
(trognlien@llnl.gov, joseph5@llnl.gov, meyer8@llnl.gov, rensink1@llnl.gov, umansky1@llnl.gov)

# Acknowledgements to previous contributors
P.N. Brown, R.H. Cohen, D.P. Grote, A.C. Hindmarsh, L.L. LoDestro, J.L. Milovich, 
A. Pankin, G.D. Porter, and G.R. Smith, all presently or formerly at LLNL; M. McCourt, 
L.C. McInnes, and H. Zhang, ANL; J.R. Cary, A.H. Hakim, S.E. Kruger, and A. Pankin, Tech-X; 
D.A. Knoll, INEEL; D.P. Stotler, PPPL; B.J. Braams, retired, IAEA; A.Yu. Pigarov and 
R. Smirnov, UCSD; J.D. Elder, U. Toronto; M. Groth, Aalto Univ.; and R.B. Campbell, Sandia.

## References
**_UEDGE development_**   
T.D. Rognlien, J.L. Milovich, M.E. Rensink, and G.D. Porter, J. Nucl. Mat. 196-198 (1992) 347-351.  
G.R. Smith, P.N. Brown, R.B. Campbell, D.A. Knoll, P.R. McHugh, M.E. Rensink, and T.D. Rognlien, J. Nucl. Mater. 220-222 (1995) 1024.  
M.E. Rensink and T.D. Rognlien, J. Nucl. Mater. 266-269 (1999) 1180.  
T.D. Rognlien, D.D. Ryutov, N. Mattor, and G.D. Porter, Phys. Plasmas 6, (1999) 1851.  
T.D. Rognlien, M.E. Rensink, and G.R. Smith, "User manual for the UEDGE edge-plasma transport code," January 2000, LLNL Rpt. UCRL-ID-137121, lastest revision May 1, 2013.  

**_Forthon development_** 
D. P. Grote, A. Friedman, I. Haber, ``Methods used in WARP3d, a Three-Dimensional PIC/Accelerator Code'', Proceedings of the 1996 Computational Accelerator Physics Conference, AIP Conference Proceedings 391, p. 51.  
See also: http://hifweb.lbl.gov/Forthon/  

**_FACETS project_**    
J.R. Cary, J. Candy, R.H. Cohen et al., J. Phys.: Conf. Ser. 125 (2008) 012040.  
A.H. Hakim, T.D. Rognlien, R.J. Groebner et al., Phys. Plasmas 19 (2012) 032505.  
M. McCourt, T.D. Rognlien, L.C. McInnes, and H. Zhang, Computational Science & Discovery 5 (2012) 014012.  

# Release 
----------------
UEDGE is released under an LGPL license.  For more details see the
NOTICE and LICENSE files.

``LLNL-CODE-759137``
