# New theoretical Fe II template for bright quasars
## This new theoretical Fe II template can be used for fitting UV to IR (1000-10000 Angstrom) spectra of quasars.

This new Fe II template is developed using the latest Fe II atomic database of [Smyth et al. (2019)](https://ui.adsabs.harvard.edu/abs/2019MNRAS.483..654S/abstract/) within the CLOUDY C23.0 ([Chatzikos et al. 2023](https://ui.adsabs.harvard.edu/abs/2023RMxAA..59..327C/abstract/)) photoionization code with the following set of parameters.

### H-ionizing photons flux: 17 $\leq \log \Phi_{\rm H}\ (\rm cm^{-2} s^{-1}) \leq$ 22, and    
### Gas density: 9 $\leq \log n_{\rm H}\  (\rm cm^{-3}) \leq$ 14
### Step size: 0.25 on log scale. 
### A fixed Hydrogen column density: 10 $^{24}$ cm $^{-2}$   
### Abundance: solar
### SED shape: standard "agn.sed", a continuum similar to  [Mathews & Ferland (1987)](https://ui.adsabs.harvard.edu/abs/1987ApJ...323..456M/abstract/)
### The Fe II template is available for the microturbulence values 0,10, 20, 30, 50 and 100 km/s.

## There are two directories; one consists of templates for only total Fe II emission while the other has templates for the outward and inward Fe II emission for different microturbulence values. 
They are named as follows.   
<img src='folder_syntax.png' alt="directory naming" style="height: 100px; width:150px;"/>

The files within each directory are named as follows:   
<img src='./file_name.png' alt="template naming">

where (a) log value of the H-ionizing photon flux in $\rm cm^{-2} s^{-1}$,    
(b) log value of the Hydrogen gas density in $\rm cm^{-3}$, and     
(c) the value of microturbulence in km/s.  

## Each template file has two columns    
<b>First column:</b> wavelength in Angstrom with 2 Angstrom binning    
<b>Second column:</b> Fe II line intensity (in erg $\rm cm^{-2} s^{-1}$)

## Templates in {\color {red} Templates_including_outward_Fe2} has four columns.
<b>First column:</b> wavelength in Angstrom with 1000 logarithmic bins between 1000 and 7000 Angstrom
<b>Second column:</b> Total Fe II line intensity (in erg $\rm cm^{-2} s^{-1}$)
<b>Second column:</b> Inward Fe II line intensity (in erg $\rm cm^{-2} s^{-1}$)
<b>Second column:</b> Outward Fe II line intensity (in erg $\rm cm^{-2} s^{-1}$)

## No Fe II emission was obtained for the following set of parameters.     

| $\log \Phi_{\rm H}$ | $\log n_{\rm H}$ |
|-------------------|----------------|
|   21.25  | 9.00 |
| 21.50  | 9.00 |
| 21.50  | 9.25 |
| 21.75  | 9.00 |
| 21.75  | 9.25 |
| 21.75  | 9.50 |
| 22.00  | 9.00 |
| 22.00  | 9.25 |
| 22.00  | 9.50 |
| 22.00  | 9.75 |

### Note: These set of parameters are for all the microturbulence velocities except zero. In case of no microturbulence velocity in addition to the upper parameters, Fe II emission was not obtained for $\log \Phi_{\rm H}$= 22 and $\log n_{\rm H}$= 10.
