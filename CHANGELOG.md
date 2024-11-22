# Changelog

Every notebook and weight file added/modified/removed from this repo will be documented in this file.

We adhere to the layout of ["Keep a Changelog"](https://keepachangelog.com/en/1.1.0/), and we follow [Semnatic Versioning](https://semver.org/). 

**Note:** Iceberg ASV transitioned to using YOLOv8 for the summer competion of Njord Challenge 2024. This notebook will start tracking versions from then.


## [2.0.0] - 2024-11-20

### Added
* Description: Added weight and notebook file for version 2 of YOLOv8
* Dataset Information: [November 20 2024 Adding Testing Annotations - No Augmen.](https://universe.roboflow.com/icebergasv/roboboat-marine-objects/dataset/2)
  * Source Details: Testing Rosbags `oct5/1969-12-31-21-22-12` and `oct5/1969-12-31-21-30-14`. Raw Rosbags in `Iceberg ASV Rosbag SSD.`
  * Preprocessing: Auto-Orient - Applied, Resize: Stretch to 640x640
  * Augmentations: No
  * Forked Source: NA
  * Cloned Source:  NA
    * Image Range: NA
    * Annotations Included: NA
  * Annotations Information:
    * Technique: Auto-labelling and manual revision of labels. Some images had a bounding box with the buoy reflection on the water.
    * Changes: NA

## [1.1.0] - 2024-11-20

### Changed
* Changed saving format of notebooks to Marine Markers Custom Dataset to it's acronym MMCD.

## [1.0.0] - 2024-10-04

### Added
* Description: Added weight and notebook file for version 1 of YOLOv8
* Dataset Information: [Buoys and Markers V3 2024-02-08 No Augmentations New Date of Feb 8 - Fork Fork](https://universe.roboflow.com/icebergasv/roboboat-marine-objects/dataset/1)
  * Source Details: All Rosbags from the Robobot 2024 Competition. Raw Rosbags in `Iceberg ASV Rosbag SSD.`
  * Preprocessing: Auto-Orient - Applied, Resize: Stretch to 640x640
  * Augmentations: No
  * Forked Source: [Old Iceberg ASV Workspace](https://universe.roboflow.com/icebergasv-ab2fn/roboboat-2024-marine-markers/dataset/3)
  * Cloned Source:  NA
    * Image Range: NA
    * Annotations Included: NA
  * Annotations Information:
    * Technique: NA
    * Changes: NA 
