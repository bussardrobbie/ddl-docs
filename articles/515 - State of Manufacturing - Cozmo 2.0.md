# State of Manufacturing: Cozmo 2.0

Hello! Digital Dream Labs has taken feedback from customers and community members regarding the need for more consistent, open communication on its current hardware manufacturing projects. Here, we'll cover the current state of **Cozmo 2.0.** Since the hardware is somewhat similar, many of the updates here will be similar to the updates for Vector 2.0.

We will strive to update these articles weekly. In some cases, there may be no new information to post; however we'll communicate everything we can, when we can. It's our objective to ensure that you have a thorough understanding of your order's status, how we are handling production and shipping, and clear up a few FAQs regarding Pre-Orders and shipment.

---

## Update as of 11/2/2022:

### **Development Unit Production:**

We have completed and successfully tested the Over the Air (OTA) update system that will allow new software to go directly onto the robot. This allows us to produce units for internal development teams to use for the later stages of app and software development. Those units are now in production.

**Self Charging (Docking):**

We are also working to ensure that Cozmo will return to dock and charge when his battery is low! One thing we haven't been clear about previously is that Cozmo 2.0 will now be an always-on robot. This is a significant difference from the first generation of Cozmo (which was limited to only being powered on when attached to a mobile device). This also means that he will need software to find and dock with his charger that he did not have before, and is one of the current items we are working to tackle.

**Cozmo's Cube (2.0):**

Each of Cozmo's 3 cubes are programmed with unique software to help Cozmo identify and interact with them! In case you have an older Cozmo, these new cubes will not work with the current generation of robots; however we still do offer Gen1 Cozmo replacement cubes! One of our current challenges is that with the differences in hardware (and operation) between Cozmo 1.0 and Cozmo 2.0, we must design a new system of connecting to all of the Cubes at once, while being mindful of how much power each Cube is using when Cozmo is interacting with them.

## ---

## Update as of 8/2/2022:

**FCC Compliance Testing:**
 [Cozmo 2.0 has FCC approval!](https://apps.fcc.gov/oetcf/eas/reports/ViewExhibitReport.cfm?mode=Exhibits&RequestTimeout=500&calledFromFrame=N&application_id=Sl8tgLtbPx6SL%2Fig6b1ecQ%3D%3D&fcc_id=2A653-00402) 🎉

---

## Update as of 7/28/2022:

**FCC compliance testing:**
 FCC compliance testing on Cozmo 2.0 has been completed by an independent laboratory. Additional testing is required for Cozmo 2.0's Cube due to changes to the electronic board for the new Cubes.

 **Software:** Software development also continues for Cozmo 2.0. Since much of the hardware has changed to streamline manufacturing, multiple changes are need to happen for the software to work correctly. However, having the hardware development completed makes this process significantly easier.

---

## Update as of 5/20/2022:

Recently, because much of the hardware is similar, a lot of the updates to Vector 2.0 also apply to Cozmo 2.0; please [see this article](//support.digitaldreamlabs.com/article/516-state-of-manufacturing-vector-2-0) to see the majority of the recent updates for base firmware for the new hardware. We are currently working on adjusting Cozmo's software to get him ready for your home! As our efforts continue, we will have more news for Cozmo specifically.

---

## Update as of 3/31/2022:

**Factory in China Reopened:**

 The contract manufacturer has reopened after the most recent COVID lockdowns in China and the factory is now back in operation. Our engineers have had several extensive meetings with factory engineers to bring them up to speed on current developments with calibration, along with providing updated documentation and instructions.

**Battery Testing:** Optimization for the battery has been delayed by work on the camera calibration. It was necessary to resolve the camera issues first as our team needs the prototypes to be able to pick up cubes, recognize faces, etc., in order to fully simulate standard usage and be able to more accurately gauge how our optimizations are affecting the new batteries.

**Camera Hardware Changes:**

 Several customers had questions on the model of camera included with Cozmo 2.0 that our team wanted to address. Previously, it had been expected that we were moving to a 5MP camera. Our team did a full investigation of the involvement this change would require, and ultimately we made the decision to revert to the 2 MP camera. This decision was made to avoid changes that would have been required to the PCB (electronics headboard) of the robot, which would have caused further delays. Thankfully, the issues that our team initially experienced with the 2MP camera have been resolved and the results of the 2MP camera are what you see below in this update.

**Changes to Display Cover:**

 With the new calibration and distortion reduction, we no longer have to make changes to the display cover! See the section below for more details.

**Camera Calibration:**

 Over the past few days, we were able to make good strides for the camera calibration. Previously, we were focusing on cleanup passes and the lighting in the calibration fixture to correct issues with the calibration. With that resolved, the last major hurdle we have been working to overcome was distortion in the camera image. Since the calibration values are hard-coded into the robot, it is a tedious process to modify these values between testing iterations. However, we've had a large breakthrough with the camera calibration process; we have narrowed down issues with distortion in the camera (see photos below) and our calibration error rate is now within a standard range (meaning effectively on par with Vector Gen 1, or within standard parameters expected for the robot to consider this no longer an issue). In the photos below depicting the distortion, you can see a significant reduction in distortion, which allows the robot to recognize fiducials (icons) on the cubes, as well as to provide better facial recognition and object recognition. This may need more testing on a batch of prototypes, but as long as results stay consistent, this breakthrough effectively resolves the camera calibration issue and it will no longer be a blocker to production.

#### 2MP Camera Adjustment Reference Photos (Distortion / Lighting)

![2MP Camera Reference Photos (After Distortion Cleanup)](//d33v4339jhl8k0.cloudfront.net/docs/assets/5e3f0b1e2c7d3a7e9ae777f5/images/6245facbab585b230a8a736f/file-LnZRGJzdBu.png)

GIF for better comparison between the two photos:

![Distorted | Undistorted Calibration Images](//d33v4339jhl8k0.cloudfront.net/docs/assets/5e3f0b1e2c7d3a7e9ae777f5/images/624606dfc1688a6d26a7befd/file-0XHJK3x5fq.gif)

---

## Update as of 3/18/2022:

**Lockdowns in China delay work by (at minimum) 1 week:** A [COVID outbreak in China](https://time.com/6157720/china-stealth-omicron-covid-outbreak/) has led to a delay of 1 week, at minimum. Strict measurements are taking place in China to stop the spread of the Omicron variant; invariably, this means that factories and business offices are shut down- while we can communicate with some members of the factory staff remotely, this slows progress and there is very little we can do to overcome that challenge given the circumstances.

**Occlusion in vision with new camera necessitates changes to the display cover:**
 In the update on 2/21/2022, an occlusion or blockage can be seen on the right hand side of the image. This occlusion is caused by the plastic display cover, which needs to be adjusted to fully utilize the field of view of the new camera.

**Testing is ongoing for the new camera calibration:**
 The new camera picture has been cleaned up fully and we are now re-testing and refining the new calibration results to ensure that calibration is heavily repeatable with a low margin of error.

**Battery Testing:**
 Power and battery measurements and refinements are continuing. The team is testing battery runtimes and charging times across multiple conditions and activity loads for the robot.

---

## Update as of 3/5/2022:

**Battery Testing**: Power optimization and testing is ongoing; no new information at this time.

**Camera Calibration**: Calibration finalization is ongoing; we are currently focusing on clarity & resolution. Additional cameras are en route and should be received on 3/8.

---

## Update as of 2/21/2022:

We are investigating some necessary software changes for calibration of the new camera module for Cozmo, and optimizing both color and resolution of the new camera to ensure that the camera's feed captures colors accurately and has face and object recognition dialed in correctly. Below, see before and after images from when we initially got the new camera working with the existing hardware modules, along with Pass 1, Pass 2, and Pass 3 of improvements for clarity and color.

### Camera Calibration

|  |  |
| --- | --- |
| **Reference Image** (*Taken with smartphone.*) | **Initial Image signal received from new camera module** (this was taken several months ago)  Issues:   1) Color   2) Clarity & Resolution   3) Duplication of image |

|  |  |
| --- | --- |
| **Cleanup Pass 1** | **Cleanup Pass 2** |

|  |  |
| --- | --- |
| **Cleanup Pass 3** (current view)  We have a bit more cleanup on the camera side for color- once those final optimizations are done, then we're good to go with this new camera! Let's move on to the current progress with the battery. |  |

## Battery

Our team's calculations showed that we should get at or slightly more than an hour of runtime on a new 600mAh battery, which is a significant jump from the previous battery which had a runtime of about 30-40 minutes. Currently, we're averaging about 52-53 minutes. There are some power optimizations we can make in multiple areas to reach our 1-hour goal. We're currently doing further testing of these optimizations.

## Software

Cozmo's software is currently being adjusted to work with some of the new hardware. We are finalizing the software additions for:

- Cliff sensors
- Display
- Camera

Once the above software changes are finalized, we should be all set to ramp production up for more units.
