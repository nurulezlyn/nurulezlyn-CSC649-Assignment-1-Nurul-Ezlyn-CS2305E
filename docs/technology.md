# Specialized Technology: Computer Vision (YOLO Object Detection)

This page summarises the specialized technology chosen for this project which is computer vision, using YOLO (You Only Look Once) object detection. It was chosen because tray checking means looking at many instruments and counting them, which an object detection model can do from a single image.

## What it is
Computer vision is a part of artificial intelligence that lets computers get useful information from images. Modern systems use deep learning, mainly convolutional neural networks (CNN), which learn visual features such as edges, shapes and textures from data instead of using hand-written rules (Sapkota et al., 2025). This project uses **object detection**, because the system must locate and count several instruments in one image.

## How it works (basic)
In supervised object detection, each training image is labelled with bounding boxes and a class for every object. The model learns to output a box, a class and a confidence score for each object it finds. YOLO (You Only Look Once) is a single-stage detector. It predicts boxes and classes in one pass, which makes it fast (Ramos & Sappa, 2025; Sapkota et al., 2025).

## Workflow in this project
Tray image (upload) → YOLO model (detect and classify) → count per instrument type → compare with tray checklist → report (Missing / Extra / OK)

## Main methods and tools
| Method / Tool | Used for in this project |
|---|---|
| YOLO (You Only Look Once) | Main model for detecting and classifying instruments on the tray. |
| Convolutional neural network (CNN) | Core of YOLO for extracting image features. |
| Precision, recall, mAP | Measuring how accurately the model detects and classifies instruments. |
| Ultralytics library | Training, validation and inference of YOLO models. |
| OpenCV | Reading and resizing images and drawing bounding boxes. |

## Benefits
- Detects and counts instruments faster than manual counting.
- Not affected by human tiredness.
- Annotated images help staff check the result.

## Limitations and risks
- Needs many labelled images across different instrument types and conditions, so data collection is time-consuming.
- Accuracy can drop when instruments look similar or overlap.
- Hospital images must be handled safely to protect private information.
- Wrong results are a risk, so the system supports staff and does not replace them (Poomrittigul et al., 2026).
- Training needs suitable hardware, which adds cost.

## Alternative considered
Manual counting with a count sheet and a second person to verify. It needs no new technology and is already accepted, but it is slow and depends on human attention. Computer vision with YOLO is chosen because it targets the slow and error-prone parts of counting.

See [references](references.md) for sources.