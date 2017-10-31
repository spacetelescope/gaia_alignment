# Gaia Alignment
This repository contains tools used for aligning HST images to Gaia.  This workflow is especially good for large mosaics/datasets multiple points but little to no overlap.  Currently, an example workflow is contained in a Jupyter notebook, though more notebooks/scripts may be added later in order to provide a more complete drizzling workflow.

The code currently provides functionality to determine the query region, 
perform the query, and pass the resulting catalog into TweakReg.  
Examples querying other services (such as MAST and DSS images) are also 
included.  The notebook uses a small subset of data from a larger HST 
program as an example, but the process is very scalable.  The full 
program was mosaicked using the same process:

![alt text](images/N44_WFC3_reduced.jpg "N44 WFC3 UVIS F814W F555W")

## Requirements
To run this notebook successfully, you will need an astroconda environment running Python (2.7 hsould work, but the code was written in 3.5).

You will also need to install the astroquery package:

`$ conda install -c astropy astroquery`
