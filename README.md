# Computer Vision Engineer Roadmap (2026)

An expanded roadmap that builds on the KDnuggets roadmap (see [roadmap_01.md](roadmap_01.md)). That one starts at geometry and goes straight to foundation models, 3D and edge. This version adds the earlier steps it skips (Python, classical image processing, core tasks) and the practices that make the work employable (data, evaluation, MLOps).

Suggested pace: about 12 months part-time. Each phase ends with a project to put on GitHub.

## Phase 0: Programming and math foundations (1-2 months)

- Python, NumPy, Git, basic C++ (needed later for performance and embedded work)
- Linear algebra, calculus, probability and statistics
- **Project:** implement convolution and image transforms from scratch in NumPy

## Phase 1: Classical image processing (1 month)

- Image formation, color spaces, filtering, edge detection
- Features (SIFT, ORB), Hough transforms, template matching
- OpenCV
- **Project:** panorama stitcher or document scanner

## Phase 2: Geometry and multi-view vision (1-2 months)

- Camera models, calibration, coordinate frames, projective geometry
- Epipolar geometry, stereo, structure from motion
- Resources: Hartley & Zisserman, *Multiple View Geometry*
- **Project:** stereo depth estimation pipeline

## Phase 3: Machine learning and deep learning (2 months)

- ML basics: overfitting, regularization, metrics
- PyTorch, CNNs, transfer learning, data augmentation
- Resources: Stanford CS231n
- **Project:** image classifier fine-tuned on a custom dataset

## Phase 4: Core CV tasks (2 months)

- Detection (YOLO family), segmentation, pose estimation, tracking, OCR
- Metrics: mAP, IoU, F1
- Dataset work: labeling, cleaning, splits, handling imbalance
- **Project:** detection plus tracking on video, evaluated with proper metrics

## Phase 5: Transformers and foundation models (1-2 months)

- ViT, Swin, CLIP/SigLIP, Grounding DINO, SAM 2
- Fine-tuning vs. zero-shot, vision-language models
- Generative models (diffusion) as awareness-level topics
- **Project:** zero-shot detection and segmentation demo across several domains

## Phase 6: 3D vision and neural rendering (1-2 months)

- Point clouds, voxels, SDFs
- Monocular depth (Depth Anything), NeRF, 3D Gaussian Splatting, SLAM
- **Project:** 3D reconstruction from video

## Phase 7: Deployment, optimization and MLOps (2 months)

- Quantization, pruning, distillation
- ONNX, TensorRT, OpenVINO, NVIDIA Jetson, DeepStream
- Docker, REST/gRPC serving, experiment tracking, CI, monitoring and drift
- **Project:** FP32 vs. INT8 benchmark, then serve the model behind an API

## Phase 8: Portfolio and career

- 3-5 polished projects, each with a README, results table and demo
- Reproduce a paper, or contribute to open source (OpenCV, Ultralytics, Hugging Face, Kornia)
- Read recent papers from CVPR, ICCV and ECCV
- Pick a specialization: robotics/autonomy, medical imaging, AR/VR, industrial inspection, or edge AI

## What this adds over the KDnuggets roadmap

| Gap in the original | Added here |
| --- | --- |
| Assumes programming and math | Phase 0 |
| No classical vision | Phase 1 |
| No core task coverage (detection, tracking, OCR) | Phase 4 |
| No data or evaluation practice | Phase 4 |
| Deployment stops at edge optimization | Phase 7 adds serving and MLOps |
| No career guidance | Phase 8 |

## Sources

- Vinod Chugani, [The Roadmap to Becoming a Computer Vision Engineer in 2026](https://www.kdnuggets.com/the-roadmap-to-becoming-a-computer-vision-engineer-in-2026), KDnuggets (basis for Phases 2, 5, 6, 7)
- Scaler, [Computer Vision Roadmap 2026](https://www.scaler.com/blog/computer-vision-roadmap/) (phased beginner path)
- GUVI, [Computer Vision Engineer Skills](https://www.guvi.in/blog/computer-vision-engineer-skills/) (six-step path: foundations, image processing, ML/DL, core tasks, MLOps, portfolio)
- Analytics Vidhya, [A Comprehensive Learning Path to Master Computer Vision](https://www.analyticsvidhya.com/blog/2020/01/computer-vision-learning-path/) (math, Python, OpenCV, ML/DL)
- Udemy, [Computer Vision Mastery 2026](https://www.udemy.com/course/computer-vision-mastery-2026opencvyolo-pytorch-projects/) (classical CV topic list)

Note: I only had search-result snippets of the secondary sources, not their full text. Several are marketing-oriented. The time estimates and the project suggestions are my own synthesis.
