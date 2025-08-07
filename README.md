# endomet_recog
endometriosis object recognition using YOLOv11 &amp; pytorch
image sourced: https://universe.roboflow.com/diagnosis/endometriosis-detection-2

The dataset includes 408 images.
Infection-rVMw are annotated in YOLOv11 format.
80 epochs, 14 batch size, 800 image size

The following pre-processing was applied to each image:
* Auto-orientation of pixel data (with EXIF-orientation stripping)
* Resize to 640x640 (Stretch)

The following augmentation was applied to create 3 versions of each source image:
* Random brigthness adjustment of between -22 and +22 percent
* Random Gaussian blur of between 0 and 2.2 pixels

> Future directions (future commits)
> 1. Less modification in preprocessing (specifically, no blur adjustment)
> 2. Using https://universe.roboflow.com/diagnosis/endometriosis-detection-jgjyx (more images, fewer classes)
> 3. Starting from this trained model instead of yolo11s.pt to improve accuracy

