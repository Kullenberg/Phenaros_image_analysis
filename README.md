# Phenaros segmentation and image analysis

This is my solution to the task given to me (https://github.com/pharmbio/SegMine). I have set up a CellProfiler pipeline (see CellProfiler_for_Phenaros_plate_96.cppipe) to segment the cells into masks, extract their morphological information (cell area, nucleus area, cell eccentricity, nucleus eccentricity, cell location, nucleus location, cell median radious and nucleus median radius) and then calculate the median values per well/site combo. The results of this are then used to make a UMAP projection by running the attached Jupyter notebook.
## Installation
To run this project, install the requirements by running `pip install -r requirements.txt`, as well as installing CellProfiler from the official website (https://cellprofiler.org/releases).

## Usage of CellProfiler
The CellProfiler pipeline requires you to open the Cellprofiler file in this repo and manually input the images corresponding to the wells used in the plate with the barcode "PB000096", which are the following:

B03, B15, C07, C22, D08, D14, D16, E03, E23, F02, F09, F13, G06, G12, G14, H08, H11, H17, H19, I21, I23, J04, J08, K07, K13, K17, L02, L10, L14, M04, M18, M20, N12, N23, O05, O10, O17, O22. 
  
In total this corresponds to 380 files, which are available for download from my google drive: (https://drive.google.com/drive/folders/1bTBKT-YwxMNIJHjGPhw9t9m8-XRmoMi1?usp=drive_link).

## Output of CellProfiler and usage of the Jupyter notebook
Running the CellProfiler pipeline will produce five .csv files with the prefix "PhenData_", a copy of which are already added to this repo for your convenience. These are then used together with the plate metadata in the attached Jupyter notebook to produce a UMAP projection.

## An example of the UMAP projection and some comments
All in all I would say there is a separation between almost all of the positive and negative controls in the final analysis, as well as a difference between the two positive controls.

![bild](https://github.com/Kullenberg/Phenaros_image_analysis/assets/169141280/6defad72-a190-4fcd-b35e-e40d238fa006)
