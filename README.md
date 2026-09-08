Hi there 👋, I'm Revaz Benidze

I'm currently finishing my bachelor's in Computer Science at Constructor University
in Bremen, Germany, with a minor in Global Economics and Management. I'm looking for
a research position or an engineering role in computer vision and 3D perception.

My bachelor thesis, built for Constructor University's autonomous racing team, is a
camera-only stereo pipeline that reconstructs metric 3D racetrack boundaries for
downstream MPC path planning, targeting the A2RL autonomous racing league at Yas
Marina Circuit.

## Current Focus

- Stereo depth estimation and metric 3D reconstruction from camera data alone, without LiDAR at inference time.

- Understanding how supervision quality shapes model behaviour: my thesis found that fine-tuning a stereo network on sparse LiDAR-derived ground truth improved aggregate error while making it measurably worse on the thin structures the task actually needed.

- Instance segmentation for thin, fragmented targets such as painted road markings, where small mask shifts dominate overlap-based scores.

👯 I'm looking to collaborate on open-source projects in computer vision, robotics perception, or machine learning.

📫 How to reach me: rbenidze@constructor.university

## CONNECT WITH ME

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/revaz-bennidze/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:rbenidze@constructor.university)

## LANGUAGES AND TOOLS

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

**Machine Learning & Computer Vision**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

**Data, Sensors & Web**

![ROS](https://img.shields.io/badge/ROS%202-22314E?style=for-the-badge&logo=ros&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

**Tools & Platforms**

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![CUDA](https://img.shields.io/badge/CUDA-76B900?style=for-the-badge&logo=nvidia&logoColor=white)

## CORE COMPETENCIES

**Computer Vision:** Stereo disparity estimation with RAFT-Stereo, instance
segmentation with RF-DETR, and geometric unprojection from disparity to metric
3D coordinates.

**Machine Learning:** Training and fine-tuning deep models in PyTorch, including
CNN architectures such as ResNet, transfer learning, data augmentation and
test-time augmentation. Focused on honest held-out evaluation, checkpoint
selection by validation metric, and diagnosing why a model fails rather than only
that it does.

**Sensor Data Engineering:** Decoding and time-synchronising multi-sensor ROS 2
recordings from MCAP, including camera and LiDAR streams publishing at different
rates. LiDAR-to-camera projection with SE(3) extrinsics, pinhole intrinsics and
distortion correction across ROS REP-103 and OpenCV frame conventions, and
building ground truth from projected LiDAR point clouds.

**Systems Programming:** Unix systems programming in C, including process
control with fork/exec, pipelines, I/O redirection and signal handling.

**Web & Databases:** Full-stack development in PHP and MySQL, with normalised
indexed schemas, prepared statements against SQL injection, session-based auth
with bcrypt-hashed credentials, and responsive front-ends in HTML5, CSS3 and
JavaScript.

**Engineering Practice:** Reproducible pipelines with recorded evaluation splits,
configuration separated from code, and documentation that states limitations
rather than hiding them.

## 🚀 Projects

### Camera-Only 3D Racetrack Border Detection ([Camera-Line-3D-detection](https://github.com/rbenidze/Camera-Line-3D-detection))

Bachelor thesis. A stereo pipeline that reconstructs metric 3D racetrack
boundaries from camera data alone, with no LiDAR at inference: RF-DETR for 2D
boundary masks, RAFT-Stereo for dense disparity, then geometric unprojection to
metric 3D points. Achieved 70.2% mAP@50 on held-out detection and a median 3D
error of 21.9 cm on the DrivingStereo holdout.

The most useful result was a negative one. Every fine-tuning run beat the
pretrained baseline on aggregate disparity error while getting measurably worse
on thin structures, because sparse LiDAR supervision lands on large planar
surfaces and teaches the network to smooth away exactly the painted lines the
task depends on. The pretrained model is the one deployed.

**Technologies:** Python, PyTorch, OpenCV, Open3D, ROS 2 / MCAP, RAFT-Stereo, RF-DETR

### A Minimal Unix Shell in C ([mysh](https://github.com/rbenidze/mysh))

A shell built from scratch with fork/exec, supporting pipelines, I/O
redirection, background jobs and signal handling.

**Technologies:** C, POSIX

### Bremen Housing Price Predictor ([bremen-housing-price-predictor](https://github.com/rbenidze/bremen-housing-price-predictor))

A machine learning model that predicts current and future housing prices in
Bremen, Germany.

**Technologies:** Python, scikit-learn, pandas

### CIFAR-10 Image Classification ([CIFAR10_Image_classification](https://github.com/rbenidze/CIFAR10_Image_classification))

A deep learning project classifying CIFAR-10 images across 10 categories,
covering preprocessing, training and evaluation.

**Technologies:** Python, PyTorch, Jupyter

## LANGUAGES

English (C1) · German (B1) · Georgian (native)
