# steRimol

An R implementation of the Sterimol parameterization process in a manner that isolates user-defined molecular subunits and does not account for non-covalently bonded units. 
The computation relies on Verloop’s original definitions [1] and begins with a user-defined bond axis, with an origin atom and a directional atom, which define the L axis. 

The function includes two atomic radii models: 
Truhlar's [2] radii, which are provided across the periodic table. 
CPK radii that are based on Paton's [3] implementation (serve as default, but are limited to main group elements). 
To use CPK radii, the workflow utilizes an open babel [4] based file conversion to include the atom types needed. 

To execute with the provided example (reproduce published results):
  1. Download all files to the same location. 
  2. Set the working directory to that location (source file location). 
  3. Run code - an Excel sheet with the computed values will be saved in the same location (in .csv format).

*** Dependencies  - The installation of the following packages is needed  ***
    
   1. data.table
   2. diversitree
   3. dplyr
   4. igraph
   5. knitr
   6. matlib
   7. plyr
   8. pracma
   9. stringr
   10. tibble
   11. tools
  
[1] A. Verloop Drug Design, Academic Press, New York, 1976

[2] J Phys Chem A, 2009 May 14;113(19):5806-12

[3] https://github.com/bobbypaton/Sterimol

[4] https://github.com/openbabel/openbabel/releases
  
