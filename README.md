Details of respiratory motion resistant DCE-MRI and DW-MRI acquisition methods and analysis of the data described below have been published recently [1, 2]. 
Under “Representative Preclinical Datasets from 9.4T” tab, a DATA folder contains 3 subfolders which were obtained from the same mouse at baseline (day0) then day7 and day14:
- KPC-27583-Pre (data from day0 pretreatment), 
- KPC-27583-Post-1 (day7) 
- KPC-27583-Post-2 (day14)

The MRI protocol is to stage the tumor size (by T2W) followed by DW-MRI and DCE-MRI in the same imaging session on day0 and day7 while only tumor size and DW-MRI on day14. Hence the day0 and day7 folder contains three subfolders while the day14 folder contains only two subfolders.  
- “DCE” subfolder includes “images” and “analysis” folders with the contents described below:
  - images (all files in compressed NIFTI format: nii.gz)
    - AFI (actual flip angle imaging) with two TR values (TR1 and TR2) for B1 mapping
    - VFA (variable flip angle) imaging for T1 mapping of the tissue using 6 flip angles: 2, 5, 8, 12, 16 and 20 degrees. 
    - DCE series: DCE images divided into timepoints 1-50, 51-100, 101-150, and 151-157.	
  - analysis (all in nii.gz format except for label description file)
    - B1 maps
    - T10 maps
    - Parametric maps of Ktrans and ve. 
    - DCE_Labels.csv: Table containing labels for each value in the DCE mask.

- “DWI” subfolder includes “images” and “analysis” folders with the contents described below:
  - images 
    - DWI.bval: b-values in standard format (space-delimited).
    - DWI.bvec: 3D vectors for direction of diffusion gradient for each b-value in standard format (space- and line-delimited).
    - DWI.nii.gz: Diffusion weighted images.
  - analysis (all in nii.gz format except for label description file)
    - Masks defined for tumor, skeletal muscle, and phantom(s)
    - ADC maps
    - KurtosisIndex maps 
    - DWI_Labels.csv: Table containing labels for each value in the DWI mask. 

- “T2” images subfolder includes the “images” folder with the contents descirbed below: 
  - images 
    - T2W.nii.gz (axial T2W images in compressed NIFTI file format)


REFERECES
1. J. Cao, H.K. Song, H. Yang, V. Castillo, J. Chen, C. Clendenin, M. Rosen, R. Zhou, S. Pickup, Respiratory Motion Mitigation and Repeatability of Two Diffusion-Weighted MRI Methods Applied to a Murine Model of Spontaneous Pancreatic Cancer, Tomography : a journal for imaging research 7(1) (2021) 66-79.
2. S. Pickup, M. Romanello, M. Gupta, H.K. Song, R. Zhou, Dynamic Contrast-Enhanced MRI in the Abdomen of Mice with High Temporal and Spatial Resolution Using Stack-of-Stars Sampling and KWIC Reconstruction, Tomography : a journal for imaging research 8(5) (2022) 2113-2128.

<!-- ![image](https://user-images.githubusercontent.com/513672/208968374-939c6ab7-6a4d-42e7-a3b6-86d6fcbcd48f.png) -->

