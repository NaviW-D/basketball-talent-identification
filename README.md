
# Basketball Tracking Project (BasketTracking)

![Logo](resources/logo_large.png)

---

## Project Overview

In professional basketball teams, tactical analysis and game statistics are essential parts of performance evaluation. This project was developed to optimize and accelerate that process using an automated **Computer Vision** system.

We designed a system capable of tracking player movements and understanding in-game events during a basketball match. The system combines classical computer vision techniques with deep learning models such as **Detectron2** to:

* Extract player trajectories
* Rectify player positions onto a standard basketball court (via homography transformation)
* Identify which player is in possession of the ball

> **Note:** Some components of this project (such as ball detection) are implemented using classical computer vision techniques like Template Matching.

---

## Demo

A demonstration video showcasing player tracking and system performance can be viewed here:

[Watch Demo Video](https://www.youtube.com/watch?v=PEziTgHx4cA)

---

## Requirements

The following libraries are required to run this project:

* **Python**
* **OpenCV** (for image processing)
* **Detectron2** (for object detection)
* **PyTorch + CUDA** (for hardware acceleration)
* **NumPy** and **Matplotlib**

---

## Usage Guide & Project Structure

The system runs through the main file:

```bash
python main.py
```

### Key Files and Their Roles

* `main.py`
  Initializes classes and loads rectified images.

* `video_handler.py`
  Handles reading frames from the input video.

* `rectify_court.py`
  Generates homography matrices, corrects court perspective, and creates panoramic views.

* `ball_detect_track.py`
  Performs automatic ball detection and tracking.

* `player_detection.py`
  Detects and tracks players.

* `player.py`
  Contains the `Player` class for managing player attributes and states.

* `tools/`
  Utility and helper functions.

* `resources/`
  Contains template images and input videos.

---

## Installation & Execution

First, clone the repository:

```bash
git clone https://github.com/NaviW-D/ml-colorization-project.git
cd ml-colorization-project
python main.py
```
