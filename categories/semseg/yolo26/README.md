# YOLOv26 (Ultralytics)

**YOLO v.26** is a new You Only Look Once (YOLO) model introduced in January 2026, which is marginally lighter, faster, and more accurate than previous versions.
Compared to the previous versions, it removes components that complicate deployment and is optimized for CPU, GPU, and NPUs.

![YOLO26](yolo26.jpg "")

## 🧠 How Does it Work?

**YOLO v.26** adds modifications by introducing transformer blocks, regression heads, and post-processing pipelines.
While traditional YOLO models depend on processes to remove duplicate bounding boxes (NMS), YOLOv26 introduces a One-to-One detection head, enabling the model to directly predict a fixed set of object hypotheses.
Additionally, it removes processes for improved bounding box precision (DFL) and replaces it with a simplified regression head, making it far easier to deploy on platforms like Jetson Orin and Raspberry Pi.

## 💡 Applications

It covers a wide range of applications in classic computer vision systems, mobile robotics, various devices, and embedded systems.

## 🚥 Limitations

Note that while **Depth Pro** provides highly accurate depth maps, it has various limitations, as listed below:
- Blurred subjects, like glasses
- Foggy and cloudy scenes
- Mirror reflections
- Graffiti illusions
- Video input (generates inconsistent and flickering depth throughout frames - Check [DepthCrafter](https://github.com/tencent/depthcrafter) for a video depth estimator)

## 🚀 Benchmark

You can find the benchmark results of **Depth Pro** for depth estimation [here](depth-pro.ipynb).
You can also find some implemented applications by **Depth Pro** [here](depth-pro-applications.ipynb).

## 📍 Links

- **🌐 Source**: [https://learnopencv.com/yolov26-real-time-deployment/](LearnOpenCV)
- **🔗 GitHub**: [https://github.com/ultralytics/ultralytics](https://github.com/ultralytics/ultralytics)
- **📄 Paper**: [https://doi.org/10.48550/arXiv.2509.25164](https://doi.org/10.48550/arXiv.2509.25164)