# csi_data

&emsp;&emsp;This project is a time series five-category data set based on received signal strength ( RSS ) readings. The dataset contains five RSS data types : one pedestrian, two pedestrians, one bicycle, two bicycles and one vehicle. The data acquisition device is composed of ESP32 and SX127x. ESP32 is a WiFi chip with a frequency of 2.4 GHz, and SX127x ( x represents 6 and 8 ) is used to generate and receive wireless signals of 915 MHz and 433 MHz.

&emsp;&emsp;In the 'dataset with different frequency and antenna height' folder, the CSV file's name includes information about the frequency and antenna height.The number before the underscore represents the antenna height, and the number after the underscore indicates the frequency.The unit of height is meter. 
`Example: 2.0_915.csv means antenna height = 2 m, frequency = 915 MHz.`

&emsp;&emsp;At the beginning of each row of data in the csv file, there is a number to distinguish different detection objects, where 1,2,3,4,5 represent one pedestrian, two pedestrians, one bicycle, two bicycles and one vehicle, respectively.
