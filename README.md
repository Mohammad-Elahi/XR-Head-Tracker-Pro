# [Head Tracker Pro](https://github.com/Mohammad-Elahi/MetaQuest_XRHeadTracker_Pro)

## Overview
Head Tracker Pro is a professional research tool developed at [the Vodafone Chair for Mobile Communications Systems at TU Dresden.](https://www.vodafone-chair.org/)

This Android NDK C++ application leverages the [Meta OpenXR SDK](https://developers.meta.com/horizon/downloads/package/oculus-openxr-mobile-sdk/) to capture and log head-tracking data from Meta Quest headsets, featuring real-time Passthrough visualization. 

This app collects head-tracking information while allowing users to maintain awareness of their physical surroundings through the Quest's Passthrough technology. The application stores motion data as a CSV file directly on the device, providing researchers and developers with easy access to movement analysis while maintaining the visual context of the real-world environment.



## Demo
https://github.com/user-attachments/assets/55aaed45-5ab6-4722-95a9-365fe2d8367e

**Now available on the [Meta Quest Store](https://www.meta.com/experiences/28111394221781002/)**

---
## Key Features:
1. Real-time head tracking
2. Passthrough visualization
3. CSV data export

Note: After exiting the app, you must restart the headset. Once restarted, you can find the CSV file in the Download folder.

## Build Instructions

### Prerequisites
- **Android Studio** (Koala or newer recommended)
- **Android NDK** (Side-by-side) installed via Android Studio SDK Manager
- **CMake** installed via Android Studio SDK Manager

### Steps to Build
1. Open Android Studio.
2. Select **Open** and navigate to the `Projects/Android` folder in this repository.
3. Wait for Gradle to sync the project.
4. If prompted to install NDK or CMake, accept the prompt.
5. Connect your Meta Quest headset via USB (ensure Developer Mode is enabled on the headset).
6. Click the **Run** button (green play icon) in Android Studio to build and deploy the APK directly to the headset.

Alternatively, to build via command line:
```bash
cd Projects/Android
./gradlew assembleDebug
```
The APK will be generated in `Projects/Android/build/outputs/apk/debug/`.

---

## Author

Mohammad Elahi, Research Assistant at Vodafone Chair for Mobile Communications Systems, TU Dresden, mohammad.elahi@mailbox.tu-dresden.de

## How to Cite

If you use this software in your research, please cite it as follows:
Elahi, M. (2024). XR Head Tracker Pro: A professional research tool for head-tracking data collection with Meta Quest headsets. GitHub: https://github.com/Mohammad-Elahi/XR-Head-Tracker-Pro

For BibTeX:

```
@software{Elahi2024XRTracker,
  author = {Elahi, Mohammad},
  title = {XR Head Tracker Pro: A professional research tool for head-tracking data collection with Meta Quest headsets},
  year = {2024},
  publisher = {GitHub},
  url = {https://github.com/Mohammad-Elahi/MetaQuest_XRHeadTracker_Pro},
  institution = {Vodafone Chair for Mobile Communications Systems, TU Dresden}
}
```
