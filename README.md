# D2Go 

D2Go is a production ready software system from FacebookResearch, which supports end-to-end model training and deployment for mobile platforms.

## What's D2Go

- It is a deep learning toolkit powered by [PyTorch](https://pytorch.org/) and [Detectron2](https://github.com/facebookresearch/detectron2).
- State-of-the-art efficient backbone networks for mobile devices.
- End-to-end model training, quantization and deployment pipeline.
- Easy export to TorchScript format for deployment.

## Installation

Install PyTorch Nightly (use CUDA 10.2 as example, see details at [PyTorch Website](https://pytorch.org/get-started/)):

```bash
conda create --name d2go python=3.8
conda install pytorch torchvision cudatoolkit=10.2 -c pytorch-nightly
```

Install Detectron2 (other installation options at [Detectron2](https://github.com/facebookresearch/detectron2/blob/master/INSTALL.md)):

```bash
python -m pip install 'git+https://github.com/facebookresearch/detectron2.git'
NB: Use double quotes on Windows OS
```

Install mobile_cv:

```bash
python -m pip install 'git+https://github.com/facebookresearch/mobile-vision.git'
NB: Use double quotes on Windows OS
```

## Get Started

```bash
python demo.py --config-file keypoint_rcnn_fbnetv3a_dsmask_C4.yaml --input tennis1.jpg --output tennis_output1_2.jpg
```

