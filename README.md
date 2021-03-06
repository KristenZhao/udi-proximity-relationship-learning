## udi-proximity-relationship-learning
Code for the paper: [Urban Data Integration Using Proximity Relationship Learning for Design, Management, and Operations of Sustainable Urban Systems.](https://doi.org/10.1061/(ASCE)CP.1943-5487.0000806)

## supporting_functions.py

This file contains the functions that are called by the relationship_learning.py. Most of the functions in this file are supporting the geometric and relationship learning algorithms written in the main code. This file shold be present in the same directory as 

## relationship_learning.py
This file contains code for preprosessing the data and learning relationships. First the data from the element files( .xlsx) is loaded into memory and then the relationship learning algorithms are executed in the following order:

-between polygon and linear elements <br>
-between polygon and polygon elements<br>
-between polygon and point elements<br>

-between point and linear elements<br>
-between point and point elements<br>
-between linear and linear elements<br>
<br>
The code only works with Python 2.x. It does not work with Python 3.x
## min_bounding_rect.py 
This file contains the code to find the minimum-area bounding box of a set of 2D points. This is a third-party supporting file which was not developed by the authors. Please see the file for more information.

## qhull_2d.py 
This file contains the code to compute the convex hull of a set of 2D points. This is a third-party supporting file which was not developed by the authors. Please see the file for more information.

## Requirements.txt
The file contains the addional packages which are needed to run the code. The use can use use this file to automatically install them. 

## Data files

The Data folder contains the data files on which we test our framework. The folder contains the following 4 sub-folders:

-Polygon --> contains all polygon element files<br>
-Linear --> contains all linear element files<br>
-Point --> contains all point element files<br>
-Block --> contains one file each (containing segments of corresponding linear elements) for all linear element files<br><br>
 
Files contained in the sub-folders are extracted from [Palo Alto open dataset](http://xmap.cityofpaloalto.org/OpenGisData/)<br>
Links to the respective datasets:<br>
[Buildings](https://fusiontables.google.com/DataSource?docid=1qgVzuCFPBv-ODQjEYEu9a1qLpdGuuycZZJjUEH9H#rows:id=1)<br>
[Trees](https://fusiontables.google.com/DataSource?docid=1XKUADil8qq1PT6xkJV3FF9bqLAZj2tBXwTTI_rc#rows:id=1) <br>
[Streets & Blocks](https://fusiontables.google.com/DataSource?docid=1Vn90L7N-dm434ts-EpWAwR7r44u8VVRAf3xoHHFX#rows:id=1)<br>

## Results of the script
The Results after running the program are stored in the "Result" folder in working directory which as a sub-folder structure similar to the Data folder

The program can only read .xlsx files right now.
