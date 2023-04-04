# Effect of urbanisation on ground beetle colour morph frequencies

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7737152.svg)](https://doi.org/10.5281/zenodo.7737152)

This repository contains all data and code needed to re-do the analyses and figures in our manuscript

"Shifts in colour morph frequencies along an urbanisation gradient in the ground beetle *Pterostichus madidus*"  

(by Maxime Dahirel, Hélène Audusseau, Solène Croci)

(link to bioRxiv preprint: https://doi.org/10.1101/2023.03.31.535151)

data in `.csv` format are in the `data` folder, R script in `.Rmd` format (including detailed information about the analysis) in the `R` folder.

This folder is a RStudio project folder, and the script uses the `here` package (see also [here](https://github.com/jennybc/here_here)) to ensure all files paths are relative. If you run the script for the first time, models and some other time-consuming outputs will be saved in the `R_output` folder so you don't have to re-run them everytime.

The file `FIG1_source.JPG` is an uncropped copy of the image that was used to make **Figure 1** of the paper.

**Important note**

A raster named `IMD_2006_020m_eu_03035_d03_E30N20.tif` is attached along public releases of the present repository on GitHub (**If reading this README from Zenodo**: assets attached to releases are not archived to Zenodo alongside the release; please go to https://github.com/mdahirel/pterostichus-morphology-2004/releases to get the file, or see next paragraph how to get it from the original source). To be able to run the entirety of the code in this repo (specifically `01-get_buffer_info.Rmd`), a copy of that raster **must** be moved to `data/GIS_layers`, with an unchanged filename. Note that data outputs based on this raster are already saved in the repo (`data/processed_data/urban_info_IMD.csv`), so failure to do this will not impede attempts to re-run most of the code (`02-analyse_data.Rmd` or `03-supplementary_material.Rmd`). 

This raster is an unmodified copy of the file of the same name made available on the EU Copernicus website (https://land.copernicus.eu/pan-european/high-resolution-layers/imperviousness/status-maps/2006 [valid link at the time of commit]). This file is made available here according to the conditions set in the Copernicus data and information policy Regulation (EU) No 1159/2013 of 12 July 2013 (see https://land.copernicus.eu/faq/about-data-access and http://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32013R1159). The use of these raster data in the present project does not imply endorsement by the European Union. These data remain the sole property of the European Union.
