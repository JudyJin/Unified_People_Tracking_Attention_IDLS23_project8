# Unified_People_Tracking_Attention_IDLS23_project8

This repository consists of individual Github repositories mentioned in the files.
The object detection is done on Roboflow and inference is made on the BoTSoRT repository.

The outputs from BoTSoRT is passed onto the attention module for gaze detection.

This is the first of a kind pipeline which incorporates face and body detection capabilities, re-identification capabilities and gaze detection capabilities into a single pipeline.
 
## Abstract
This project presents a novel framework that utilizes one-shot object detection models to analyze classroom settings and quantify attendance, safety, and engagement of the attendees. The proposed approach has the potential to revolutionize traditional classroom attendance tracking and provide a more comprehensive assessment of classroom dynamics, thereby enabling educators to tailor their teaching methodologies to improve student learning outcomes. The framework combines deep learning and computer vision techniques to provide a scalable and accurate solution for educational purposes.

## Improvements made

- Novel Dataset Creation
- Object Detection Fine Training on Novel Dataset
- Re-Identification improvement in matching algorithm
- Re-Identification Fine Training on Novel Dataset
- Gaze Detection Fine Training on Novel Dataset
- Combination of three individual data modules into a single data pipeline

## Overall Data Pipeline

<p align="center"><img src="assets/pipeline old.png"/></p>

## Directory Structure
The attention module takes us to the attention respository which can be used to fine-tune the attention model based on the instructions.

The BoT-SORT module takes us to the re-identification repository which also contains inferences from object detection.


## Novel Dataset (Annotated and Non-Annotated)

https://drive.google.com/drive/folders/1Fb15nKbm9hvYum4F6usQyQ6uwfge87fY?usp=share_link

(Currently restricted to only Carnegie Mellon University IDs with permissions from people in the dataset)

## Requirements

See `JudyJin/Unified_People_Tracking_Attention_IDLS23_project8/combined_requirements.txt`

## Demo Video(Best Result)

https://drive.google.com/file/d/16tWfHb4biFKOynVyk-GH-liLNDO25Rod/view?usp=sharing

## Other Demo Results for Re-ID:
https://drive.google.com/drive/folders/1HtWcHifGN0EzNLz_vDgmSFvnXR1qHwsY?usp=sharing

## Usage

Can be currently used in a classroom environment for qualitatively analyzing the engagement based on ID. We want to improve this by using quantifiable metrics for attention evaluation.

## References

A large part of codes, ideas and metrics are borrowed from 
[BoT-SORT](https://github.com/NirAharon/BoT-SORT), 
[labelme](https://github.com/wkentaro/labelme),
[Yolov8 - Ultralytics](https://github.com/ultralytics/ultralytics) and
[Attention](https://github.com/ejcgt/attention-target-detection).
Thanks for their excellent work!
