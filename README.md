# RCES Final Project 
Junzhe Liu 2022

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pangeo-data/pangeo-docker-images/2022.09.21?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252FJerryLIU-Junzhe%252Frces-final-project%26urlpath%3Dlab%252Ftree%252Frces-final-project%252Frces_final_project.ipynb)

### Goal & Scientific Question

1. Examine how global Mixed Layer Depth (MLD) pattern of
my Mixed Layer Depth (MLD) algorithm similar to or different from those of existing methods.

2. Learn to process metadata in clouds with Dask. 



### Dataset - Argo 

    (1) NOAA AOML (.nc)
    https://www.ncei.noaa.gov/data/oceans/argo/gadr/data/aoml/
    or
    https://nrlgodae1.nrlmry.navy.mil/cgi-bin/argo_select.pl?startyear=2022&startmonth=11&startday=08&endyear=2022&endmonth=11&endday=16&Nlat=90&Wlon=-180&Elon=180&Slat=-90&dac=ALL&floatid=ALL&gentype=plt&.submit=++Go++&.cgifields=endday&.cgifields=dac&.cgifields=startday&.cgifields=startmonth&.cgifields=endmonth&.cgifields=gentype&.cgifields=startyear&.cgifields=endyear&.cgifields=delayed
    
    (2) Euro-Argo ERIC (.CSV)
    https://fleetmonitoring.euro-argo.eu/dashboard?Status=Active&Basin=ATLANTIC%20OCEAN
 
 

### Analysis Plan

Load Data into xarray and split each profile into Dask arrays. For each profile, get MLD with my stability method, temperature threshold method (Thompson, 1976), density threshold method (Weller and Plueddeman, 1996; Kara et,. al, 2000), Holte and talley integrated method (Holte and talley, 2009), and maximum buoyancy frequency method (Carvalhol et,.al, 2017). Examine the MLD sptial and temporal correlations between different methods. 