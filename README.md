# SWIFT-BAT-Machine-Learning-Detections
machine learning support vector model codes for original and low-res GRB and glitch data on Niel Gehrels SWIFT Observatory / Burst Alert Telescope
## Authors
Kate Foyle | Department of Astronomy and Astrophysics | Eberly College of Science | The Pennsylvania State University
#### Mentored by:
Dr. James DeLaunay | Assistant Research Professor | Department of Astronomy and Astrophysics | Eberly College of Science | The Pennsylvania State University

## Overview
This project utilizes machine learning (ML) for glitch detection -- and subsequent rejection -- in data from the Burst Alert Telescope (BAT) aboard the Neil Gehrels Swift Observatory. By training on known heat pipe glitch patterns and gamma-ray bursts (GRBs), the purpose is to improve the sensitivity of BAT's trigger system and enable a more refined search for more multi-messenger detections involving GRBs and gravitational waves (GWs). For any given trigger or signal-to-noise (S/N) ratio, machine learning reduces the false alarm rate, allowing for more confidence in GRB detections.
## Goals
- turn Swift/BAT's current glitch detection process into a machine learning method using Support Vector Machines (SVMs).

- reject a higher percentage of instrumental glitches that BAT is currently triggering on to lower the false alarm rate for any given S/N trigger.

- increase the sensitivity to faint GRBs to improve the chances of identifying multi-messenger detections between GRBs and GWs.

## Installation/Imports
pip install astropy beautifulsoup4 matplotlib numpy requests scikit-learn swifttools
## Notebooks
#### GRB_.ipynb
This notebook contains the downloading process of real GRB detector plane images (DPIs) in two resolutions from the Swift/BAT Gamma-Ray Burst Catalog. 
#### GLITCH_.ipynb
This notebook contains the process of finding heat pipe glitches in GUANO dumps and downloading their detector plane images (DPIs) in two resolutions.
#### SVM_.ipynb
This notebook conjoins the GRBs and glitches in their respective resolution and trains and tests on them with scikit-learn's SVM Support Vector Classifier (SVC) to find the 
#### use_SVM.ipynb
uploading my saved versions...
## Files
#### svm_original_model.pkl
#### svm_lowRES_model.pkl
## Citations / Acknowledgments
NASA's HEASARC, "swifttools" package by THAT GUY who owns it, https://swift.gsfc.nasa.gov/results/batgrbcat/, 

