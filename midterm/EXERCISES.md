# Exercises – Answer Sheet

### LIST OF EXERCISES

**Student name:** Diptansu Roy
**Date:** _submission date_

The exercises count for 5% of the final grade (results 2% + reflection 3%). Completing the other track as well gives a bonus of +2%.

## How to fill in this sheet

1. Choose **one** track and tick it below.
2. For each exercise in your track, give:
   - **Result:** one or two screenshots, an output file or a link that shows the exercise works.
   - **Reflection:** about half a page that answers the three questions.
3. Put your screenshots and output files in [`figures/track-a/`](figures/track-a/) or [`figures/track-b/`](figures/track-b/) and link or embed them with relative paths, e.g. `![Exercise 1](figures/track-a/ex1_result.png)`.
4. For the bonus, also fill in the section of the other track. Delete the section of a track you did not do.

## Chosen track

- [ ] **Track A – no programming:** the 5 initial exercises
- [ ] **Track B – advanced (programming needed):** cross-domain digital twin and sensor data integration
- [X] **Bonus:** I completed both tracks

---

## Track A – no programming

### Exercise A1: Visualizing existing data from AHN and 3DBAG

**Result**

![Exercise A1 result]
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/Error%20in%20Blender%20ex1.jpeg
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/Digital%20Surface%20Model%20campus%20ex1.png
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/R_34Fn2%20modified%20ex1.png.aux.xml
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/campus%20buildings%20ex1.mtl
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/campus%20buildings%20ex1.obj

**Reflection**

- **What did you do?**

In the first exercise, I downloaded AHN height data (Digital Surface Model) and 3d building data for the University of Twente Campus area and prepared the files to be visualised in Twinmotion.

After selecting the correct tiles and downloading AHN data, I processed it in TerraSculptor where I rescaled and cropped the DSM to the university campus area, compressed the image to reduce variability of height and resampled it to be used with Unreal Engine (Twinmotion). 

For the 3D building data, i downloaded it from two different tiles as the campus is not fully covered by a single one. I chose to use the LOD 2.2 model for processing as I have good computing power. In Blender, I combined both the obj files, changed their orientation to North and made sure that each object can be separated individually later on (by using loose parts tool). Finally, I exported the output as another obj file.

- **What did you struggle with, and how did you solve it?**

I was having quite a lot of trouble when fixing the orientation of the 3d bag data in Blender. Setting X,Y,Z coordinates to 0 would lead to a weird artifacting and distorted lines were created. A few of my peers were also facing this problem but none of us could understand why. After restarting blender 2-3 times, the problem went away.

- **How useful is it for your own digital twin? Will you use it in your final?**

This exercise forms the base of creating a digital twin and therefore, it will be very important for my own digital twin model. It taught me how to collect raw data and pre-process it for visualisation.

I will definitely use these steps in my final if I choose to create a digital twin within the Netherlands using 3d Bag and Elevation data.

### Exercise A2: Making a 2D building plot in QGIS and exporting it to Blender

**Result**

![Exercise A2 result]
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/Blender%20output%20Ex%202.PNG
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/Difference%20Export.rar
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/QGIS%20output%20Ex%202.PNG
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/Water%20export.rar
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/carre.rar


**Reflection**

- **What did you do?**
In this exercise, I created the 2D plot of a new builiding (with exteriors) from scratch in QGIS which I then exported to Blender where I corrected some of the geometries of the water and the building. The plot was edited in a way that the water outlet we created could be separated from the building and the inner water pool could also be disjointed from the actual building. 
- **What did you struggle with, and how did you solve it?**
Since I am quite a novice in working with Blender, I struggled a little when removing the building's faces from the water pool in between. I was also having trouble using the 'Knife Project tool to cut through the section of the building where the water had to pass through. Blender kept on giving me the prompt of 'No other selected objects have wire or boundary edges to use for projection'. To solve both these problems, I carefully went through the steps again and tried to deselect and select the faces I wanted to remove or edit. 
- **How useful is it for your own digital twin? Will you use it in your final?**
  For my own digital twin, I will most likely create it in blender. Therefore, any and all exercises using blender gives me an opportunity to use and learn the tools, making me become more familiar with how to efficiently create a model. 
  
I may not use the entire workflow of creating a shapefile in QGIS and then exporting to Blender as I prefer using ArcGIS, however I shall definitely use the methods taught to separate faces in Blender.

### Exercise A3: Creating a 3D building in Blender

**Result**

![Exercise A3 result]
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/Basic%20cube.mtl
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/Basic%20cube.obj
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/Building%20output.PNG
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/Cube%20output.PNG
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/building.fbx

**Reflection**

- **What did you do?**
In this exercise I learnt more on how to use tools to make 3d models in Blender. TI used these tools (such as subdivide, loop cuts and extrusion, uv mapping) on a cube and then later made a 3d building from the 2d shapefile created earlier . I also assigned material to the faces of the building with different colours and textures (such as shine). The exercise also focused on checking whether all your faces of the model were facing the outside or not. Without this check, some of your walls may disappear.

The 3d building I created had a outlet for the water to flow thorugh, windows, different floors and different textures for each material type (such as brown to showcase wooden frames).

- **What did you struggle with, and how did you solve it?**
 This was one of the easier exercises for me so the only thing which i struggled a little with was where to place my cursor when sub dividing or extruding to do it correctly. Sometimes the loop cuts made would be vertical instead of horizontal and so on. However, I dealt with them by simply practicing and having patience.

- **How useful is it for your own digital twin? Will you use it in your final?**
This exercise is extremely crucial in learning how to make a 3d model, therefore it remains one of the most useful things I shall use for my project. I aim to experiment more with blender to understand the tools better.

### Exercise A4: Creating a 3D road network from OSM data

**Result**

![Exercise A4 result]
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/Blender%20output%20Ex%204.PNG
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/QGIS%20Output%20Ex%204.PNG
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/buffer%201.rar
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/buffer%202.rar
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/road%20network%20clipped%20rd%20new.rar
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/road%20network.fbx
https://github.com/diptansu-roy/3D_DT_Course/commit/e6c04c3261c881fdc47e69ae3047ccb9d3807f5e

**Reflection**

- **What did you do?**
 I created a 3d model of the road network of the University of Twente campus area with QGIS and Blender. Firstly, I filtered and extracted the road network using Quick OSM and vector geoprocessing tools. I removed several attribute columns from the road types and turned them into shapefiles. The shapefiles of roads and the buffer of these roads were then exported into Blender to be converted into 3d fbx files to be used in Twinmotion later on for visualisation.

- **What did you struggle with, and how did you solve it?**
I struggled quite a bit with converting the osm data files into shapefiles due to there being too many attributes (shapfiles can only accept about 250 attributes). I thought I had deleted the extra unimportant columns from my data but the changes had not saved, so I could not understand why it was not working. I tried to convert them with a third party tool but Blender could not verify the geometry from those files. I ended up going back to QGIS and inspect each layer again where I found many of the changes I had made hadn't saved. So, I did them again and this time it worked perfectly.


- **How useful is it for your own digital twin? Will you use it in your final?**
Modelling a road network won't be quite as useful to me as I plan to focus on modelling one building accurately. However, It was quite helpful to learn on how extracting data from OSM works as I will use that for other purposes if not for my final project.

I do not think I shall use road network modelling for my final.

### Exercise A5: Using Twinmotion to Visualise Data

**Result**

![Exercise A5 result]
https://github.com/diptansu-roy/3D_DT_Course/blob/main/midterm/figures/track-a/Exercise%205%20Output%20and%20Videos

**Reflection**

- **What did you do?**
As a final culmination of all the other exercises, in this one I visualised 3d buildings, roads and the landscape using Twinmotion. The buildings, parking and roads of the University of Twente campus were loaded into Twinmotion as geometries along with my own building which I had previously modelled. All these elements were placed on top of the DSM I created in the very first exercise. Next, I tweaked the environment to add effects such as trees, grass, material on buildings, snow, rain, fog etc. I also added dynamic elements such as a cycling path and pedestrians. Finally, I exported a video showcasing my complete 3D model after troubleshooting and aligning everything.

- **What did you struggle with, and how did you solve it?**
The most trouble I faced was definitely aligning all the elements together as their pivots were not synced. Bringing them to 0,0,0 coordinates still put them afar as some had RD coordinates in them and other elements did not (like the DSM). I fixed it by centring the pivot.

Being a computationally demanding software, Twinmotion also crashed making me lose some progress. Therefore, I did some of the steps twice and tried to reduce my graphics setting so that the software doesn't crash again.

- **How useful is it for your own digital twin? Will you use it in your final?**
Twinmotion provides a very flexible and user friendly way to demonstrate your 3d model and I deem it quite useful for my project. I shall definitely use it to showcase my final output, using it to develop more of the background scene and textures.

---

## Track B – advanced

### Exercise B1: Cross-domain digital twin

**Result**

![Exercise B1 result](figures/track-b/b1_result.png)

_Optional: link to your code, an output file or an online result._

**Reflection**

- **What did you do?**
  _Your answer here._
- **What did you struggle with, and how did you solve it?**
  _Your answer here._
- **How useful is it for your own digital twin? Will you use it in your final?**
  _Your answer here._

### Exercise B2: Sensor data integration

**Result**

![Exercise B2 result](figures/track-b/b2_result.png)

_Optional: link to your code, an output file or an online result._

**Reflection**

- **What did you do?**
  _Your answer here._
- **What did you struggle with, and how did you solve it?**
  _Your answer here._
- **How useful is it for your own digital twin? Will you use it in your final?**
  _Your answer here._
