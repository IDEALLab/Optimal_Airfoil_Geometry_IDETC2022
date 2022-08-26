Machine learning models and 2D airfoil dimensionality reduction code associated with our accepted IDETC 2022 paper: "Effect of Optimal Geometries and Performance Parameters on Airfoil Latent Space Dimension." Paper is accessible via: https://ideal.umd.edu/papers/paper/idetc-vansloot-optimized-geomerty-airfoil 


# Notebooks
#
## OPT_AE_DIM.ipynb
 - Uses both PCA and Autoencoder models for dimensionality reduction on the Optimized Airfoil Data Set
 - Calculates training and testing MSE vs latent space size for 1-20 dimensions

#
## OPT_AE_DIM_PARAM.ipynb
 - Uses both PCA and Autoencoder models for dimensionality reduction on the Optimized Airfoil Data Set, including the performance parameters of Mach number, Reynolds number, angle of attack and target lift coefficient that were used as inputs to the SU2 adjoint solver when the airfoils were optimized 
 - Calculates training and testing MSE vs latent space size for 1-20 dimensions

#
## OPT_AE_TRAIN.ipynb
 - Uses both PCA and Autoencoder models for dimensionality reduction on the Optimized Airfoil Data Set
 - Calculates training and testing MSE vs training size for 3,4, and 5 dimensions

#
## Plotting.ipynb
 - Plots the data

#
## UIUC_AE_DIM.ipynb
 - Uses both PCA and Autoencoder models for dimensionality reduction on the Non-Optimized Airfoil Data Set (UIUC airfoil database)
 - Calculates training and testing MSE vs latent space size for 1-20 dimensions

#
# Data
## initial
### airfoil_interp_192.npy
- This dataset consists of 1528 airfoils taken from the UIUC airfoil database
- Each airfoil consists of 192 x and y coordinates
- Referred to as 'UIUC data set'
### airfoils_opt.npy
- The optimized airfoils dataset (2D coordinates) with the highest efficiency (Cl/Cd) under corresponding boundary conditions
### aoas_opt.npy
- The optimized angle of attack of each optimized airfoil
### inp_paras.npy
- The input boundary conditions (Mach number, Reynolds number, and target lift coefficient) to the SU2 adjoint optimizer used to create airfoils_opt

# Note
Training and testing data frames output from autoencoder models were too large to upload to github directly. These files can be accessed through https://drive.google.com/drive/folders/18FP8GZM1-1ZmK6rE5tW4OFlhb2tw5In0?usp=sharing rather than via /data/generated
