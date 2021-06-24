# FURA-2 Analysis [![DOI](https://zenodo.org/badge/373477639.svg)](https://zenodo.org/badge/latestdoi/373477639)

This script is in 2 parts, the first working on ImageJ/Fiji and the second is using VBA (Excel).
The second part is available as .vba files (the code itself to include into your notebook) or as .xlsm files (the Excel file itself) where you only have to press on the button "start script" (the .xlsm file need to be in the same folder as the data).

/!\ READ documentation within the script before use.  
Here is a summary of the instructions.

### First Script (ImageJ/Fiji)
Put all the images into a folder named "1_Images".  
Add an identification at the beginning of each dish name in the format: "Dishxxx" (the capital letter is important).  
Create 2 set of ROIs to put in a folder named "2_ROIs", 1 for background subtraction and 1 for the cells to measure:
- with the corresponding identification "Dishxxx" ending with _BG		(Capital letters are important)
- with the corresponding identification "Dishxxx" ending with _cells	(no capital letter)

### Second Script (VBA)
Two versions are available, one to create a ratio of 2 channels (FURA-Analysis_2) and another one to just work with 1 channel data (FURA-Analysis_2_MnQuench).  
The ratio version works only for files containing either "340" or "380" in their name, you could modify these two identification parameters (lines 31 and 32, var names "IdFile1" and "IdFile2") to make a ratio of any set of files.  
The 1 channel version works only for files containing "360" in their name, you could modify this value to open any file (line 27, var name "IdFile1").
