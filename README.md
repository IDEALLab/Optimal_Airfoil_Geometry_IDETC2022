Machine learning models and 2D airfoil dimensionality reduction code associated with our accepted IDETC 2022 paper: "Effect of Optimal Geometries and Performance Parameters on Airfoil Latent Space Dimension."


# notebooks
#
## OPT_AE_DIM
 - Uses both PCA and Autoencoder models for dimensionality reduction on the Optimized Airfoil Data Set
 - Calculates training and testing MSE vs latent space size for 1-20 dimensions

#
## OPT_AE_DIM_PARAM
 - Uses both PCA and Autoencoder models for dimensionality reduction on the Optimized Airfoil Data Set, including the performance parameters of Mach number, Reynolds number, angle of attack and target lift coefficient that were used as inputs to the SU2 adjoint solver when the airfoils were optimized 
 - Calculates training and testing MSE vs latent space size for 1-20 dimensions

#
## OPT_AE_TRAIN
 - Uses both PCA and Autoencoder models for dimensionality reduction on the Optimized Airfoil Data Set
 - Calculates training and testing MSE vs training size for 3,4, and 5 dimensions

#
## Plotting
 - Plots the data

#
## UIUC_AE_DIM
 - Uses both PCA and Autoencoder models for dimensionality reduction on the Non-Optimized Airfoil Data Set (UIUC airfoil database)
 - Calculates training and testing MSE vs latent space size for 1-20 dimensions

#
# data
## initial
### airfoil_interp_192
- This dataset consists of 1528 airfoils taken from the UIUC airfoil database
- Each airfoil consists of 192 x and y coordinates
- Referred to as 'UIUC data set'
### airfoils_opt
- The optimized airfoils dataset (2D coordinates) with the highest efficiency (Cl/Cd) under corresponding boundary conditions
### aoas_opt
- The optimized angle of attack of each optimized airfoil
### inp_paras
- The input boundary conditions (Mach number, Reynolds number, and target lift coefficient) to the SU2 adjoint optimizer used to create airfoils_opt
