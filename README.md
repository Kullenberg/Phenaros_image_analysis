# Phenaros_image_analysis

This is my solution to the task. I have set up a CellProfiler pipeline (see CellProfiler_for_Phenaros_plate_96.cppipe) to segment the cells into masks, extract their morphological information (cell area, nucleus area, cell eccentricity, nucleus eccentricity, location and median radious) and the calculates the median values per image.
The CellProfiler pipeline requires you to manually input the images corresponding to the wells used in the plate with the barcode "PB000096", which are the following:

  B03, B15, C07, C22, D08, D14, D16, E03, E23, F02, F09, F13, G06, G12, G14, H08, H11, H17, H19, I21, I23, J04, J08, K07, K13, K17, L02, L10, L14, M04, M18, M20, N12, N23, O05, O10, O17, O22. In total this corresponds to 380 files.

  This will produce the five .csv files with the prefix "PhenData_", which are then used together with the plate metadata in the attached Jupyter notebook.
  This produced the image "UMAP_projection.png" also attached in this Github repo. 

  All in all I would say there is a separation between the positive and negative controls in the final analysis, as well as a difference between the two positive controls.
  


![UMAP_projection](https://github.com/Kullenberg/Phenaros-Task/assets/169141280/896b2311-552e-4bc7-8693-e0e4cc3941d3)
