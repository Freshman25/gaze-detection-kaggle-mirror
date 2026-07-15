# gaze-detection-kaggle-mirror
This repository provides a mirrored copy of the Gaze Detection dataset from Kaggle for research, experimentation, and machine learning development. It preserves the original dataset structure to simplify reproducibility and integration into computer vision pipelines. I am the author of the data.

## Tested Platforms
| Platform | OS | Hardware | Status |
|----------|----|----------|--------|
| Ubuntu 22.04 | Ubuntu 22.04 LTS | NVIDIA GPU (CUDA) | ✅ Passed |
| macOS | macOS Tahoe | CPU | ✅ Passed |

## Architecture & Design
The repository uses a small **Adapter Pattern** that provides a common interface for object detection models. This allows the same dataset, training loop and evaluation pipeline to work across different frameworks.
training loop and evaluation pipeline to work across different frameworks.
<ul>
  <li>torchvision.models.detection (PyTorch)
    <ul>
      <li>Faster R-CNN</li>
      <li>RetinaNet</li>
    </ul>
  </li>
  <li>AutoModelForObjectDetection (Hugging Face)
    <ul>
      <li>RT-DETR</li>
    </ul>
  </li>
</ul>
