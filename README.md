# Reconstruction-of-LST-images-using-MSSA
Reconstructing Daytime and Nighttime MODIS Land Surface Temperature Using Multi-Channel Singular Spectrum Analysis

You can download files including images, codes and MSSA from the following link:
https://www.dropbox.com/scl/fi/upd8spvop07moasjtbsk5/MSSA_LST.rar?rlkey=yix4mvhyw2xxecfgztb5fi9ab&st=mry1mh38&dl=0

The following actions are required to reconstruct the land surface temperature images of MODIS sensor:
In the image folder: day and night images of the Land surface temperature product for a time series are placed, which can be downloaded from the following sites:
https://appeears.earthdatacloud.nasa.gov/
https://ladsweb.modaps.eosdis.nasa.gov/
Then all the day and night images are placed in a folder respectively and its format is converted to raw. which is shown here under the folder name All_day_night_raw.
To enter the images into the MSSA software, it is necessary to convert the images into a text file, and the time series images are divided into several blocks. Choosing the number of blocks depends on the RAM of your system and the size of the area. For example, the time series can be divided into two or four blocks. To convert images into blocks, the Matlab code located in the Cod_matlab_import_export_MSSA folder with the name SSA_raw_tool is used. envi_read must be executed before executing this code. After running the code, enter the path of images with raw extension in the window that opens and enter the number of rows and columns of images and the number of desired blocks. Then the data is entered into the MSSA software. The MSSA software is installed in the Linux and the file of this software is located in the MSSA folder. After reconstructing the image with MSSA, the output of the software is converted into reconstructed time series images using the MATLAB code SSA_reconstructed_tool.
