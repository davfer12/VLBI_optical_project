# VLBI_optical_project
This is the neccesary code and data to reproduce the figures and results of the Nature Astro paper 'Detection of an orthogonal alignment between parsec scale AGN
jets and their host galaxies' (D. Fernández Gil, J. A. Hodgson, B. L’Huillier, J. Asorey, C. Saulder, K. Finner, M. J. Jee, D. Parkinson, F. Combes). 

The 'libraries.py' file imports all necessary python libraries and dependencies as of Python 3.8.

The 'data_loading_and_xmatching.py' file contains all functions pertaining to loading the catalogues, performing the cross-matches, saving them into csv files and loading them afterwards.

The 'get_catalogue_parameters.py' file contains functions that access the catalogue data and gets their relevantr parameters.

The 'aux_functions.py' file contains auxiliary functions that perform various tasks such as dealing with angles, computing the optical/VLBI angle difference, carrying out a MonteCarlo technique, obtaining statistical siognificances and handling 3D rotations for the Eagle simulation results.

The 'main_functions.py' file contains the root of the data handlin and ganalysis. It creates a combined dataset from the individual catalogues, it prepares the data for the histogram figures, obtains the p-values and plots it.

The 'figures.py' file contains functions that generate every figure of the paper.

The 'pregenerate_neccesary_data' script deals with taking the original optical catalogue data and performing a cross-match with the VLBI data, as well as taking a random sample from two of the catalogues which are used in the coverage map of Figure 2. We include this code here for transparency purposes, but the original optical catalogue data is too heavy to upload. We only upload the cross-matched outputs generated from this script in the data files. 

The 'main' script uses all other files to load the catalogues and cross-matches and execute every function to generate all the Figures.

The 'data' folder includes the whole VLBI Astrogeo data, the mentioned optical/VLBI cross-matches, the sampled optical catalogues and the Eagle simulation data.

The 'paper_figures' folder includes all the Figures of the paper. 

If the user wants to reproduce the Figures, they just have to save all these files together with the 'data' folder and run the 'main' script. The figures will be saved in the 'paper_figures' folder. 
