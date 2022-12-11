# RCES Final Project 
Junzhe Liu 2022

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pangeo-data/pangeo-docker-images/2022.09.21?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252FJerryLIU-Junzhe%252Frces-final-project%26urlpath%3Dlab%252Ftree%252Frces-final-project%252Frces_final_project.ipynb)

### Goal & Scientific Question

1. Examine consistency in results of MLD algorithms (actively using ones)

2. Learn to process metadata in clouds with Dask. 



### Dataset - Argo 

    Python Package argopy developed by euroargo program

### Analysis Plan

Load Data into xarray and split each profile into Dask arrays. For each profile, get MLD with my stability method, temperature threshold method (Thompson, 1976), density threshold method (Weller and Plueddeman, 1996; Kara et,. al, 2000), Holte and talley integrated method (Holte and talley, 2009), and maximum buoyancy frequency method (Carvalhol et,.al, 2017). Examine the MLD sptial and temporal correlations between different methods. 