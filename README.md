# Calculate the 2D number density of the MD system via the TCL function in VMD
# Place the file dc.tcl in the folder into the VMD installation directory. 
# Add the following content to the last line of the vmd.rc file:
          source dc.tcl
          cd d:/**/**
          dc NVT_system.lammpstrj(or *.pdb/xyz/dcd/psf) NVT_system.lammpstrj(or *.pdb/xyz/dcd/psf) number_xy 1000(firstFrame) 2000(lastFrame) 10(/step) 0 49.46800 30 0 53.29800 30 24 30 1 {atomSelection}

# a. mass_xy, mass_yz, mass_xz, mass_x, mass_y, mass_z are for mass density caculation;
# b. number_xy, number_yz, number_xz, number_x, number_y, number_z are for number density caculation;
# c. mass_xy calculates 2D mass density on XY plane;
# d. while number_x calculates 1D number density along X axis
# xl xh xr yl yh yr zl zh zr
       
