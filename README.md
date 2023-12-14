The code is set up to run on my machine and there may be absolute file paths that will not work on other machines. 

The flow for the code here can be seen much better in the Youtube video linked in the submission. 

A lot of the images are gitignored as otherwise the git repository would overshoot its maximum storage limit very quickly. 

The flow of the code is as follows:

use the s3 sync command to pull images from aws.

create a new assets folder and paste all the images from the selected experiment into that folder - this is very manual and the way to do it is look at the date on the image in your OS's file system structure.

copy the opencv1 file and name it with the experiment number - make sure to go through and check that all the input and output folders have also had their names changed - then run the script

this will move all the images into a new folder with the calculated y coordinate in front of the file name.

then go into the graphing folder and copy paste the graphs... ipynb file. This will process those file names into usable data and turn it into a csv 

then go to tempcombine and run tempcombine to see all the experiments on the same graph 

finally , run tempfitcurve to get a logistic function to fit the data - some clear outliers may need manual removal - these outliers should be checked all the way from the beginning with the images
