# Deploy CoreML on IOS for object detection

> supporting models: (https://github.com/ultralytics/yolov5), [`YOLOv5`]

![platform-ios](https://img.shields.io/badge/platform-ios-lightgrey.svg)
![swift-version](https://img.shields.io/badge/swift-4.2-red.svg)
![lisence](https://img.shields.io/badge/license-MIT-black.svg)

This project is Object Detection on iOS with Core ML.

## Requirements

- Xcode 14.x
- iOS 16.0+
- Swift 5.7.x

## How To Build and Run the Project

### 1. Clone the project

```shell
git clone https://github.com/kaiven11/coreml_for_ios
```
### 2. Add the model to the project

Rename the `ObjectDetection-CoreML.PY` file to `ObjectDetection-CoreML.xcodeproj`,and use Xcode to open it.
By default, the project uses the `yolov5s` model. 
you can use `export-nms.py` to export pt to CoreML file.
```shell
python export-nms.py --include coreml --weights yolov5n.pt
```
### 3. Set model name properly in `ViewController.swift`
### 4. Build and Run

## See also

- [motlabs/awesome-ml-demos-with-ios](https://github.com/motlabs/awesome-ml-demos-with-ios)<br>
  : The challenge using machine learning model created from tensorflow on iOS
  : YOLOv8 repository
- [ultralytics/yolov5](https://github.com/ultralytics/yolov5)<br>
  : YOLOv5 repository
