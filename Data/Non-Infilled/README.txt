This dataset is a collection of non-infilled temperature (Celsius) portraits of the Narragansett Bay from May 1984 to September 2022. The temperature data is derived from the thermal band of the Landsat 5, 7, and 8 satellites. The following steps detail how the data was downloaded and processed into its current state.

1) Access Landsat 5, 7, and 8 data using Google Earth Engine in Google Colab.
2) Access Narragansett Bay buoy data from the following website (June 2003 to November 2019).
https://data-explorer.riddc.brown.edu/dataset/ri-buoy/summary
3) Compare the overlapping buoy and Landsat data for each satellite and derive three different bias values (mean difference between the buoy and Landsat data). The bias values are -0.450 for Landsat 5, -1.094 for Landsat 7, and 0.178 for Landsat 8.
4) Subtract these bias values from the data on a satellite by satellite basis.

This dataset is data from all three satellites combined. The metadata has three columns, the first being the date of each satellite image, the second being the percent cloud cover over the Bay in the image, and the third being the satellite that captured the image. Once the data from the three satellites was combined into one large dataset, statistics were calculated for the difference between the Landsat data and the buoy data, and are reported below. When using the data, you can choose to filter by the cloud cover percentage image.

Mean: 0.320
Standard Deviation: 2.507
Skewness: 2.425
Kurtosis: 12.899