# Crowd count
## Assessment of protesters joining the march on 19th Nov 2023, in Copenhagen (Denmark).

## Method: Jacob's method applied to UAV imagery

* We estimated crowd density based on orthoimages (i.e. strictly top-down viewpoint) from UAV and the [Jacob's method](https://www.sciencedirect.com/science/article/pii/S1877705815010358). The images used to assess density are shown in dir ../**top-down_images_people_density**).
* Then, we applied the estimated crowd densities to each polygon constituting the march---during the time period 15:51 to 15:53.
* The polygons add up to the surface shown in the image file **Area_filmed_protest_1551.PNG**: 30500 m^2.

* Support information is shown in the dir .../**circumstantial_evidence**.


## Results

* The estimate following the above-mentioned method gives: **37700 +- 5000 people** were filmed during the protest on the 19th November 2023.
* This is the estimate of people filmed in the UAV-footage during the time period 15:51 to 15:53.

## counting people

* The images used to assess density are manually labeled, assisted via a regular [CNN model for object recognition](https://www.kaggle.com/code/grayphantom/counting-people-yolov3-gluoncv).
* Every image is human verified. Results are available in the dir ../**top-down_images_people_density**.
* We used  [DotDotGoose](https://biodiversityinformatics.amnh.org/open_source/dotdotgoose/). DotDotGoose is a free, open source tool to assist with manually counting objects in images.

## density estimates and assumptions

* We evaluated the density at 10 different locations based on top-down UAV-footage.

* We asusmed the densities estimated are:
  * statistically independent---they are taken at different locations and points in time.
  * Gaussian distributed around its mean (1.2 +- 0.2 people/m^2).

  **People density (people/m^2)** : we calculated densities in 2 different replicates (a,b) per density type. More information is given in dir ../**top-down_images_people_density**		

| density_type | replicate_a |replicate_b |
| :---------------- | :------: |  :------: |
| density_lowest | 0,8465 |	0,8580	|
| density_low |  0,9746	| 0,8998 |
| density_mid |  1,0394	| 1,0719 |
| density_high  | 1,1553	| 1,5508 |	
| density_highest | 1,3845 |	1,4465	|
| mean:  | 1.11 | 1.23 | 
| std: | 0.19 | 0.28  |


## 

* The people we report of are shown in the footage material (dir ..**/screenshots_footage_**). The timestamp of each screenshot is also included.

  ## Other crowds joining the protest are not filmed
* Additionally, other protesters attended directly Slotspladsen (Christiansborg palace), at the time of the footage (dir ..**/circumstantial_evidence**). These are not included in our estimate, neither the ones joining the march at any point after 15:53. 

