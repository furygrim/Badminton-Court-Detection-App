# Badminton-Court-Detection-App
# Badminton Court Detection App

An interactive application for detecting badminton courts in images and videos, hosted on Streamlit. This project implements two distinct approaches for court detection: a traditional computer vision technique using color segmentation and a deep learning approach using the YOLOv8 model.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Approaches](#approaches)
  - [Traditional Computer Vision (Color Segmentation)](#traditional-computer-vision-color-segmentation)
  - [Deep Learning (YOLOv8)](#deep-learning-yolov8)
- [Installation](#installation)

## Overview

The Badminton Court Detection App is designed to detect badminton courts from various input images and videos. It leverages two main approaches:
1. **Traditional Computer Vision:** Uses color segmentation to distinguish court boundaries and key features based on color differences.
2. **Deep Learning:** Implements the YOLOv8 model for object detection to precisely locate and classify badminton courts within a scene.

By integrating these methods into a Streamlit interface, users can easily upload images or video streams, view detection results, and compare the performance of each approach.

## Features

- **Dual Detection Approaches:** Compare traditional computer vision techniques with advanced deep learning models.
- **Real-Time Processing:** Designed for fast inference on images and video inputs.
- **Interactive UI:** User-friendly interface built with Streamlit.
- **Model Comparison:** Visualize and compare results from the color segmentation method and the YOLOv8-based detector.
- **Extensible Framework:** Modular code structure for easy updates and experimentation.

## Approaches

### Traditional Computer Vision (Color Segmentation)

This approach leverages the unique color properties of a badminton court:
- **Preprocessing:** Image enhancement and noise reduction.
- **Segmentation:** Isolates the court region by segmenting specific color ranges typical of badminton courts.
- **Post-Processing:** Refines detected boundaries using morphological operations.
- **Advantages:** Simple, fast, and computationally inexpensive.
- **Limitations:** May be sensitive to lighting conditions and background clutter.

### Deep Learning (YOLOv8)

The YOLOv8 model provides a robust object detection solution:
- **Model Architecture:** YOLOv8, a state-of-the-art real-time object detection algorithm.
- **Training:** Trained on a curated dataset of badminton court images, the model can recognize and localize courts with high accuracy.
- **Inference:** Processes images to output bounding boxes and confidence scores.
- **Advantages:** High detection accuracy and robustness against diverse image conditions.
- **Limitations:** Requires more computational resources and a larger dataset for training.

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/furygrim/badminton-court-detection.git
   cd badminton-court-detection
