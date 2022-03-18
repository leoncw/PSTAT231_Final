## README

This project was completed March 18th, 2022 for course credit for PSTAT 131/231 at the University of California Santa Barbara.<br>

If running this folder locally, a number of dependencies may need to be installed, see the libraries subsection. This project is designed to be run from RStudio. Publication of the output uses the knitr package. Stylization of the .html output relies on the development version of the rmdformats package. The development version of this package is necessary as the current stable Cran version (as of 3/18/2022) does not correctly implement code-folding when publishing to .html file.

-The raw_data folder contains data from the global environmental indicators dataset on kaggle: https://www.kaggle.com/ruchi798/global-environmental-indicators. In theory, this data could be edited in the future. Therefore a local copy is stored in raw_data, instead of directly accessing it from the project. <br>
-The crosswalks folder contains crosswalk files to match the countries from different .csv files in the raw data. <br>
-The data dictionary provides a summary of the variables used in the modeling stections from the global environmental indicators data set. <br>
-The intermediate data folder contains data saved at intermediate stages in the Final_Project_html_Broderick_Weinberg.Rmd file. <br>
-The model output folder saves some output from models that either is intensive to rerun (and hence was saved once so that the Rmarkdown knitting was not a problem) OR compiled poorly during the knitting process, but runs fine locally.<br>
-The Rmd folder contains code related to the different sections of the report. NOTE THAT THE FINAL VERSION OF THE CODE IS IN Final_Project_html_Broderick_Weinberg.Rmd, and the versions in Rmd have been slightly altered in most cases after being added to the final report<br>

Final_Project_html_Broderick_Weinberg.Rmd is the final product of this report, and is published as a knitted html file: Final_Project_html_Broderick_Weinberg.html. It is currently available online at https://leoncw.github.io/PSTAT231_Final/Final_Project_html_Broderick_Weinberg.html.<br>

If running this projectly locally, the entire folder should be downloaded. Then the following line (line 24) of Final_Project_html_Broderick_Weinberg.html should be changed to match your local directly:<br>
knitr::opts_knit$set(root.dir = "/home/clw/Documents/UCSB/Quarter6/PSTAT 231/Final Project/PSTAT231_Final")<br>

(note the above requires the knitr package and assumes the user is using RStudio)