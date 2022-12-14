## MODEL Barrois_VO_2018

### Preamble
This document is best viewed with Markdown support. _Last updated: November 2018 (Loïc Huder)_.

### Model description
Surface core flows over 2001-2017 obtained under a dynamo spatial norm with an augmented state stochastic Kalman filter [[Barrois et al. 2017](https://doi.org/10.1093/gji/ggx280)]. These are inverted directly from magnetic records above Earth's surface, namely ground-based series (GO) and virtual observatory (VO) series [[Barrois et al. 2018](https://doi.org/10.1093/gji/ggy297); [Barrois PhD thesis, 2017](http://www.theses.fr/s119100)]. 

Magnetic data have been provided by C. Finlay and M. Hammer from DTU Copenhagen. 

### Provided data
#### Measures
This model provides the Gauss coefficients of the following quantities (called thereafter **measures**):

* **Sub-grid errors (ER):** errors due to the projection onto large length-scales of subgrid (nonlinear) induction processes. Also includes the contribution of the magnetic diffusion.
* **Magnetic field (MF):** the main field
* **Secular variation (SV):** the secular variation
* **Core flow (U):**  the core flow

All these quantities are given at analysis steps.

#### File names
Each measure has a separate set of files whose names contain the measure name. 

All the individual measure realisations generated by the computation are given in their respective .zip file (`Analysed_Realisations_measureName.zip`). For convenience, .dat files containing the mean (`Analysed_mean_measureName.dat`) and the variance (`Analysed_rms_measureName.dat`) of the realisations are also provided.

#### File format
The files store the Gauss coefficients according to the following format : each line corresponds to an epoch (given as the first element) and is composed of the sequence of the Gauss coefficients at this epoch separated by simple spaces.

This gives in practice:

* For SV, MF, ER:

$` t1 \space g_{1,0}(t1) \space g_{1,1}(t1) \space h_{1,1}(t1) \space g_{2,0}(t1) \space g_{2,1}(t1) \space h_{2,1}(t1) \space g_{2,2}(t1) \space h_{2,2}(t1) \space g_{3,0}(t1) ... `$  
$` t2 \space g_{1,0}(t2) \space g_{1,1}(t2) \space h_{1,1}(t2) \space g_{2,0}(t2) \space g_{2,1}(t2) \space h_{2,1}(t2) \space g_{2,2}(t2) \space h_{2,2}(t2) \space g_{3,0}(t2) ... `$  
$` ... `$  

* For U:

$` t1 \space t^c_{1,0}(t1) \space t^c_{1,1}(t1) \space t^s_{1,1}(t1) \space t^c_{2,0}(t1) \space ... \space s^c_{1,0}(t1) \space s^c_{1,1}(t1) \space s^s_{1,1}(t1) \space s^c_{2,0}(t1) ... `$  
$` t2 \space t^c_{1,0}(t2) \space t^c_{1,1}(t2) \space t^s_{1,1}(t2) \space t^c_{2,0}(t2) \space ... \space s^c_{1,0}(t2) \space s^c_{1,1}(t2) \space s^s_{1,1}(t2) \space s^c_{2,0}(t2) ... `$  
$` ... `$  

### Citations
If the use of this data leads to any output, please cite the following references:
* Barrois, O., Hammer, M.D., Finlay, C.C., Martin, Y. and Gillet, N., 2018. Assimilation of ground and satellite magnetic measurements: inference of core surface magnetic and velocity field changes. _Geophysical Journal International_ **215**: 695-712 (https://doi.org/10.1093/gji/ggy297).

### Contact
For any inquiries, please refer to the contact information on [http://geodyn.univ-grenoble-alpes.fr].

 
