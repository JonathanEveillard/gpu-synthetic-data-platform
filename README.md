# GPU Synthetic Data Platform

A GPU powered synthetic data generation platform for training 
and validating perception AI. Inspired by Parallel Domain.

## What This Is
Real world sensor input, reconstructs it into photorealistic 3D simulations using NeRF and Gaussian Splatting, then generates thousands of scene variations to train computer vision models without real world data collection. Built on production grade GPU infrastructure Kubernetes, CUDA, Terraform, and full observability, with final model deployment to edge hardware.

## Architecture
TBD

## Component Projects
- [ ] Month 1-2: GPU vs CPU Benchmark
- [ ] Month 2-3: 3D Scene Reconstruction
- [ ] Month 3-4: Real-Time Object Detection
- [ ] Month 4-5: Synthetic Scene Variation Pipeline
- [ ] Month 5-6: GPU Scheduled Kubernetes Inference
- [ ] Month 6-7: GPU Observability Dashboard
- [ ] Month 7-8: Job Submission API
- [ ] Month 8-9: ML Experiment Tracker
- [ ] Month 9-10: Edge Model Deployment


## Tech Stack

### 3D Reconstruction
- COLMAP | Structure from Motion, camera pose extraction
- nerfstudio | NeRF training and novel view synthesis
- gsplat | Gaussian Splatting (replaces NeRF, month 9+)

### Scene Variation
- Blender + bpy | programmatic scene variation and rendering
- NVIDIA Omniverse | photorealistic rendering (month 7+)

### ML / AI
- PyTorch | deep learning framework, training and inference
- YOLOv8 (Ultralytics) | object detection and perception evaluation
- Depth Anything | monocular depth estimation
- MLflow | experiment tracking and model registry
- TensorRT | model optimization and quantization for edge deployment
- ONNX | model export and interoperability

### Sim-to-Real Validation
- FID Score (Fréchet Inception Distance) | synthetic data quality metric

### Sensor Hardware
- Intel RealSense D435 | RGB-D camera for real sensor input
- NVIDIA Jetson Orin Nano | edge deployment target

### Containers
- Docker + NVIDIA Container Toolkit | GPU-accelerated containerization
- CUDA 12.2 | base runtime for all GPU workloads
- GitHub Container Registry | image storage and versioning

### Orchestration
- Kubernetes | GPU

## Status
In progress | started `June 25 2026`
