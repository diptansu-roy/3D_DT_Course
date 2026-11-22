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

### Exercise A3: _name of the exercise_

**Result**

![Exercise A3 result](figures/track-a/a3_result.png)

_Optional: link to an output file or online result._

**Reflection**

- **What did you do?**
  _Your answer here._
- **What did you struggle with, and how did you solve it?**
  _Your answer here._
- **How useful is it for your own digital twin? Will you use it in your final?**
  _Your answer here._

### Exercise A4: _name of the exercise_

**Result**

![Exercise A4 result](figures/track-a/a4_result.png)

_Optional: link to an output file or online result._

**Reflection**

- **What did you do?**
  _Your answer here._
- **What did you struggle with, and how did you solve it?**
  _Your answer here._
- **How useful is it for your own digital twin? Will you use it in your final?**
  _Your answer here._

### Exercise A5: _name of the exercise_

**Result**

![Exercise A5 result](figures/track-a/a5_result.png)

_Optional: link to an output file or online result._

**Reflection**

- **What did you do?**
  _Your answer here._
- **What did you struggle with, and how did you solve it?**
  _Your answer here._
- **How useful is it for your own digital twin? Will you use it in your final?**
  _Your answer here._

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
