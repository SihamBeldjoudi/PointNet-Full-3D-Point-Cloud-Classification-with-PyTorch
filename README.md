# PointNet-Full-3D-Point-Cloud-Classification-with-PyTorch
This project implements PointNet (and simplified variants) for 3D point cloud classification using the ModelNet40 dataset.   

<img width="469" height="350" alt="image" src="https://github.com/user-attachments/assets/318e3fe4-b153-48db-a320-540cd2dc1b3b" />

## Project Overview

### Models
- **PointMLP** — a simple MLP reference model  
- **PointNetBasic** — a basic PointNet without T-Net  
- **PointNetFull** — full architecture with **Transformation Network (T-Net)** and regularization

### Key Components
- Read/write support for `.ply` point cloud files  
- `PointCloudData` dataset class for train/test split  
- Data augmentation transforms:
  - Random rotation, scaling, noise, translation, and flipping  
- Loss functions:
  - `basic_loss` for PointMLP / PointNetBasic  
  - `pointnet_full_loss` for PointNetFull (with matrix regularization)  
- `train()` function for full training & evaluation loop  




---


## Installation

### 1. Clone the repository
```bash
git clone https://github.com/SihamBeldjoudi/PointNet-Full.git
cd PointNet-Full
