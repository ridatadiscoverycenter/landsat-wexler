Contained within this download are four folders.


1) Non-Infilled: A collection of Landsat 5, 7, and 8 temperature scenes of the Narragansett Bay.
---> The scenes folder contains all of the .csv Landsat temperature scenes.
---> The metadata.csv file contains information about each Landsat scene.
---> The README.txt file contains more information about the data product


2) Infilled: A collection of Landsat 5, 7, and 8 temperature scenes of the Narragansett Bay with clouds infilled. The cloud infilling was performed using DINEOF (Beckers and Rixon, 2003).
---> The scenes folder contains all of the cloud-infilled .csv Landsat temperature scenes.
---> The metadata.csv file contains information about each Landsat scene.
---> The README.txt file contains more information about the data product.


3) Coordinates: Contains files with latitude and longitude information.
---> The latitude.csv file contains the latitude of every pixel in the Landsat scenes.
---> The longitude.csv file contains the longitude of every pixel in the Landsat scenes.


4) Notebooks: Contains the four Google Colab notebooks used to download, process, and analyze data.
---> bias_correction: Performs a bias correction of the Landsat thermal band using buoys throughout the Narragansett Bay. These bias corrections are applied to the Landsat data.
---> landsat_scenes: Downloads .csv Landsat thermal scenes of the Narragansett Bay.
---> non_infiiled: Calculates statistics for the non-infilled Landsat scenes that are reported in the README.txt file in the Non-Infilled folder.
---> infilling_dineof: Performs the DINEOF algorithm on the Landsat scenes to remove clouds.


Email daniel_wexler@brown.edu, daniel_wexler@alumni.brown.edu or danwexler32@gmail.com or baylor@brown.edu with questions.