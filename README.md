# steRimol

An R implementation of the Sterimol parameterization process in a manner that isolates user-defined molecular subunits and does not account for non-covalently bonded units. 
The computation relies on Verloop’s original definitions and begins with a user-defined bond axis, with an origin atom and a directional atom, which define the L axis. 

The function includes two atomic radii models, the default being Truhlar's [2] radii, as they are provided across the periodic table. CPK radii are also enabled and are based on 
Paton's [3] implementation. To use CPK radii, the workflow utilizes an open babel [4] based file conversion to include the atom types needed. 

To execute with the provided example (reproduce published results):
  1. Download the zip file and extract all files to the same location. 
  2. Set the working directory to that location (source file location). 
  3. Run code - an Excel sheet with the computed values will be saved in the same (in .csv format).
  
