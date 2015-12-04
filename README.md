#Instruction to install basemap and GEOS (Geometry Engine - Open Source) library,
the package (basemap-1.0.7.tar.gz) is already downloaded in the resource folder.

The below instructions come from:              
http://matplotlib.org/basemap/users/installing.html 

Step 1: If numpy 1.0.0 or later, python 2.4 or later, matplotlib 1.0.0 are installed, go to     step2, otherwise install them

Step 2: Untar the basemap-1.0.7.tar.gz file, and and cd to the basemap-1.0.7 directory

Step 3:
If you already have GEOS library on your system, just set the environment variable GEOS_DIR to point to the location of libgeos_c and geos_c.h (if libgeos_c is in /usr/local/lib and geos_c.h is in /usr/local/include, set GEOS_DIR to /usr/local). Then go to next step. 
If you don’t have it, you can build it from the source code included with basemap by following these commands in the command line:
#
cd geos-3.3.3
export GEOS_DIR= /home/ds-ga-1007  
#it is your home directory, I recommend this.
# If any permission wrong happens, use sudo su to get the super user authority, or get # root authority
./configure --prefix=$GEOS_DIR
