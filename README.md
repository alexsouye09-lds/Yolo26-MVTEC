
Real-time Industrial Defect Detection with YOLO26m

Overview

This project demonstrates a production-ready industrial defect detection system based on Ultralytics YOLO26m, deployed on edge hardware for real-time quality control.

The solution targets Automated Optical Inspection (AOI) use cases such as PCB inspection, cable assembly verification, and component defect detection, without cloud dependency.

Key Features

Real-time inference at 25 FPS @ 640×640

<40 ms latency per frame

Multi-class defect detection:

bent_lead

cable_swap

broken_small / broken_large

contamination

scratches


100% on-device processing (edge AI)

Optimized for industrial environments


Model & Training

Model: YOLO26m (Ultralytics, Jan 2026)

Optimizer: MuSGD (Multi-Scale SGD + Muon hybrid)

Loss Functions: ProgLoss + STAL (small-object optimization)

Dataset: Custom industrial defect dataset

Accuracy: >93% mAP (production-grade)


YOLO26 Innovations Used

End-to-End NMS-Free detection (lower latency)

MuSGD for faster convergence and better generalization

DFL removal for easier export and hardware compatibility

Improved small-object detection for PCB-level defects

~43% faster CPU inference compared to previous YOLO generations


Performance Summary

Metric	Value

FPS	25
Latency	<40 ms
Resolution	640×640
Deployment	Edge / Offline


Industrial Impact

~750× faster than manual inspection

Hardware cost <500 € vs 10k–50k € traditional AOI systems

Scalable to multi-camera production lines

Compatible with Industrie 4.0 / Smart Factory / MES integration


Applications

Electronics Manufacturing

PCB Inspection

Cable Assembly

Component Verification

Automated Optical Inspection (AOI)

Industrial Quality Control


Next Steps

Integration with factory MES systems

Multi-camera synchronization

Long-term production monitoring and analytics


Acknowledgments

Special thanks to Ultralytics and Glenn Jocher for the YOLO26 release and open-source vision AI ecosystem.


---

Author: Alexis Oueda
Contact: ouedaalexis@gmail.com 
