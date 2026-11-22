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

### Exercise A1: _name of the exercise_

**Result**

![Exercise A1 result](figures/track-a/a1_result.png)

_Optional: link to an output file or online result._

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

### Exercise A2: _name of the exercise_

**Result**

![Exercise A2 result](figures/track-a/a2_result.png)

_Optional: link to an output file or online result._

**Reflection**

- **What did you do?**
  _Your answer here._
- **What did you struggle with, and how did you solve it?**
  _Your answer here._
- **How useful is it for your own digital twin? Will you use it in your final?**
  _Your answer here._

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
