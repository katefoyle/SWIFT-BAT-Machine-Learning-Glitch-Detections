# SWIFT-BAT-Machine-Learning-Detections
machine learning support vector model codes for original and low-res GRB and glitch data on Niel Gehrels SWIFT Observatory / Burst Alert Telescope
## Authors
Kate Foyle | Department of Astronomy and Astrophysics | Eberly College of Science | The Pennsylvania State University
#### Mentored by:
Dr. James DeLaunay | Assistant Research Professor | Department of Astronomy and Astrophysics | Eberly College of Science | The Pennsylvania State University

## Overview
This project utilizes machine learning (ML) for glitch detection -- and subsequent rejection -- in data from the Burst Alert Telescope (BAT) aboard the Neil Gehrels Swift Observatory. By training on known heat pipe glitch patterns and gamma-ray bursts (GRBs), the purpose is to improve the sensitivity of BAT's trigger system and enable a more refined search for more multi-messenger detections involving GRBs and gravitational waves (GWs). For any given trigger or signal-to-noise (S/N) ratio, machine learning reduces the false alarm rate, allowing for more confidence in GRB detections.
## Goals
- Turn Swift/BAT's current glitch detection process into a machine learning method using Support Vector Machines (SVMs).

- Reject a higher percentage of instrumental glitches that BAT is currently triggering on to lower the false alarm rate for any given S/N trigger.

- Increase the sensitivity to faint GRBs to improve the chances of identifying multi-messenger detections between GRBs and GWs.
## Installation/Imports
pip install astropy beautifulsoup4 matplotlib numpy requests scikit-learn swifttools
## Notebooks
#### GRB_.ipynb
Downloads real GRB detector plane images (DPIs) from "The Swift/BAT Gamma-Ray Burst Catalog" in both original and low-resolution. 
#### GLITCH_.ipynb
Finds heat pipe glitch events in GUANO dumps and downloads their corresponding DPIs in both original and low resolution.
#### SVM_.ipynb
Conjoins the GRBs and glitches DPI datasets in the selected resolution and trains a scikit-learn SVM classifier to distinguish between GRBs and instrumental glitches. 
#### use_SVM.ipynb
uploading my saved versions...
## Files
#### svm_original_model.pkl
#### svm_lowRES_model.pkl
## Citations / Acknowledgments
NASA's HEASARC, "swifttools" package by THAT GUY who owns it, https://swift.gsfc.nasa.gov/results/batgrbcat/, 

