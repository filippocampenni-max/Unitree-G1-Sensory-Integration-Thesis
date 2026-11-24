# Unitree G1 Humanoid Robot – 3D Sensory Integration & Perception

![Degree](https://img.shields.io/badge/Degree-BSc%20Mechanical%20Engineering-003366)
![Grade](https://img.shields.io/badge/Grade-110%2F110%20cum%20laude-brightgreen)
![Institution](https://img.shields.io/badge/University-UNIVPM-red)
![Language](https://img.shields.io/badge/Thesis%20Language-Italian-blue)

## Document Access
📄 **[Read / Download Full BSc Thesis (PDF)](./Filippo_Campenni_BSc_Thesis_Unitree_G1.pdf)**

---

## Abstract & Project Overview
Bachelor's Thesis in Mechanical Engineering at **Università Politecnica delle Marche (UNIVPM)** — Graduated October 2026 with **110/110 cum laude**.

This work addresses the multi-sensor integration and real-time environmental perception of the **Unitree G1 EDU** humanoid robot. The project combines 3D LiDAR spatial mapping and statistical point-cloud filtering with deep-learning RGB-D object detection to enable real-time 3D target localization in unstructured environments.

## Key Engineering Highlights
* **Multi-Sensor Hardware & FOV Integration:** Analyzed the geometric mounting constraints and overlapping Field of View (FOV) between the **Livox Mid-360** 3D LiDAR and the **Intel RealSense D435i** RGB-D camera on the Unitree G1 platform.
* **3D LiDAR Point-Cloud Post-Processing:** Acquired raw spatial point clouds during dynamic mapping sessions and implemented automated **Python** post-processing pipelines applying *Statistical Outlier Removal* (SOR) filters (**Open3D**, **PyVista**) to eliminate dynamic operator trails and sensor noise prior to 3D SLAM relocalization.
* **Real-Time RGB-D Object Detection:** Integrated the Intel RealSense D435i depth stream with **Ultralytics YOLOv11** via **ROS 2 Humble** on Ubuntu Linux to compute real-time 3D spatial coordinates $(X, Y, Z)$ of detected targets.
* **Custom Dataset & Model Validation:** Built and augmented a custom dataset (891 base images, 3x augmentation via Roboflow), achieving **0.886 mAP@0.5** and an **F1-score of 0.87**.
* **Kinematic Telemetry & SDK Integration:** Interfaced with **Unitree SDK2** (C++/Python) to manage sensor coordinate-frame transformations and hardware telemetry.

## Hardware & Software Stack
* **Hardware:** Unitree G1 EDU Humanoid Robot, Livox Mid-360 3D LiDAR, Intel RealSense D435i RGB-D Camera.
* **Software & Frameworks:** Ubuntu 22.04, ROS 2 Humble, Python, Ultralytics YOLOv11, Open3D, PyVista, Unitree SDK2.

## Thesis Structure (Italian Manuscript)
1. **Introduction & Objectives:** Context of humanoid robotics and sensory perception requirements.
2. **Hardware Architecture:** Mechanical and electronic overview of the Unitree G1 EDU, Livox Mid-360, and RealSense D435i.
3. **Software & Communication Stack:** Network configuration, Unitree SDK2, and ROS 2 Humble middleware architecture.
4. **3D Object Detection Pipeline:** Dataset creation, Roboflow augmentation, YOLOv11 training, live object detection and coordinate estimation.
5. **3D SLAM & Point-Cloud Filtering:** Spatial mapping experiments and Statistical Outlier Removal filtering.
6. **Conclusions & Future Developments:** Summary of experimental results and sensor-fusion perspectives.
