Pole Creek fire WRF-SFIRE version

[![DOI](https://zenodo.org/badge/281750493.svg)](https://zenodo.org/badge/latestdoi/281750493)
<br><br>

SFIRE - Spread fire model in WRF-Fire<br>
<br>
*** Jan Mandel August 2007 - March 2011 <br>
*** email: Jan.Mandel@gmail.com<br>
<br>
For support please go to <br>
http://www.openwfm.org/wiki/WRF-Fire_user_support <br>
<br>
Current user's guide can be found at<br>
http://www.openwfm.org/wiki/Users_guide <br>
<br>
For reference publications see<br>
http://www.openwfm.org/wiki/WRF-Fire_publications<br>
<br>
A limited version from 2010 is included in WRF release. We no longer <br>
support that version.<br>
<br>
This module is the only entry point from WRF-ARW to the wildland <br>
fire model. The call to sfire_driver advances the fire model by <br>
one timestep. The fire model inputs the wind and outputs <br>
temperature and humidity tendencies. The fire model also inputs a <br>
number of constant arrays (fuel data, topography). Additional <br>
arguments are model state (for data assimilation) and constant arrays <br>
the model gives to WRF for safekeeping because it is not allowed <br>
to save anything.<br>
<br>
This code as of mid-2011 is described in [1]. If you use this code, <br>
please acknowledge our work by citing [1].<br>
Thank you.<br>
<br>
Acknowledgements<br>
The fire physics code is adapted from the CAWFE code [2].<br>
The coupling with WRF is adapted from a code by Ned Patton, <br>
coupling a Fortran 90 port of the CAWFE fire module to WRF [3].<br>
Support of refined fire grids in WRF was provided by John Michalakes.<br>
Jonathan D. Beezley has set up and maintained the WRF build and<br>
execution environment, provided software engineering infrastructure <br>
including synchronization with the WRF repository, and was responsibe<br>
for all aspects of WRF modification. UCD students Minjeong Kim and<br>
Volodymyr Kondratenko have contributed to the implementation of the<br>
fire propagation by the level set method.<br>
<br>
Refefences<br>
[1] Jan Mandel, Jonathan D. Beezley, and Adam K. Kochanski, "Coupled
atmosphere-wildland fire modeling with WRF 3.3 and SFIRE 2011, 
Geoscientific Model Development (GMD) 4, 591-610, 2011. 
doi:10.5194/gmd-4-591-2011<br>
<br>
[2] T. L. Clark, J. Coen, and D. Latham, Description of a coupled 
atmosphere-fire model, Intl. J. Wildland Fire, vol. 13, pp. 49-64, 
2004<br>
<br>
[3] Edward G. Patton and Janice L. Coen, WRF-Fire: A Coupled 
Atmosphere-Fire Module for WRF, Preprints of Joint MM5/Weather 
Research and Forecasting Model Users' Workshop, Boulder, CO, 
June 22-25, 2004, pp. 221-223, NCAR<br>
<br>
! --------------------------------------------------------------------<br>
! <br>
! CURRENT ACTIVITY<br>
! <br>
! For current activity and development trends please check out<br>
! http://ccm.ucdenver.edu/wiki/User:Jmandel/blog<br>
! http://www.openwfm.org/wiki/WRF-Fire_development_notes<br>
! <br>
<br>
<br>
ADDITIONAL DOCUMENTATION IN THE doc SUBDIRECTORY<br>
<br>
<br>
README.txt                  this file<br>
README_git.txt              how to use the versioning system<br>
README_mac.txt              how to run on a Mac<br>
README_matlab_netcdf.txt    how to read WRF input and output directly in Matlab<br>
README_vis.txt              matlab visualization using files written every timestep<br>
README_visualization.txt    convert WRF input and output to Matlab<br>
README_wps.txt              how use real data including fuel from Landfire<br>
<br>


