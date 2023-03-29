This dataset is a collection of cloud-infilled temperature (Celsius) portraits of the Narragansett Bay from May 1984 to September 2022. The temperature data is derived from the thermal band of the Landsat 5, 7, and 8 satellites. The cloud infilling was performed using the DINEOF (Data Interpolating Empirical Orthogonal Functions) algorithm developed by Beckers and Rixon, 2003. The following steps detail how the data was downloaded and processed into its current state.

1) Access Landsat 5, 7, and 8 data using Google Earth Engine in Google Colab.
2) Access Narragansett Bay buoy data from the following website (June 2003 to November 2019).
https://data-explorer.riddc.brown.edu/dataset/ri-buoy/summary
3) Compare the overlapping buoy and Landsat data for each satellite and derive three different bias values (mean difference between the buoy and Landsat data).
4) Subtract these bias values from the data on a satellite by satellite basis. The bias values are -0.450 for Landsat 5, -1.094 for Landsat 7, and 0.178 for Landsat 8.
5) Perform the cloud-infilling DINEOF algorithm on the three datasets separately, using only scenes with less than 80% cloud cover over the Bay in the process (this means that there is no infilled data for Landsat scenes with more than 80% cloud cover over the bay). This excludes 226 scenes.

This dataset is cloud-infilled data from all three satellites combined. The metadata has three columns, the first being the date of each satellite image, the second being the percent cloud cover over the Bay in the original, non-infilled image, and the third being the satellite that captured the image. Once the data from the three satellites was combined into one large dataset, statistics were calculated for the difference between the infilled data and the buoy data, and are reported below. When using the data, you can choose to filter by the cloud cover percentage of the original, non-infilled image.

Mean: 0.670
Standard Deviation: 3.277
Skewness: 1.252
Kurtosis: 6.550