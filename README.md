# 🔬 Towards High-Resolution 3D Reconstruction in Volume Electron Microscopy

The project aims to build a **full-pipeline image processing platform for Volume Electron Microscopy (VEM)**，enabling automated stitching, alignment, restoration, reconstruction, and segmentation of high-resolution, large-scale biological 3D structures.
Built upon the team’s series of research contributions published in top-tier venues such as **NeurIPS, AAAI, ACM Multimedia, and GigaScience**，this project seeks to deliver a **reproducible, extensible, and interactive** VEM processing toolkit.

---

## 📌 Background

Volume Electron Microscopy (VEM) is a revolutionary biological imaging technology, recognized by *Nature* as one of the **“Seven Technologies to Watch in 2023”**. It enables nanoscale-resolution visualization of the three-dimensional structures of cells, tissues, and even small organisms.

However, the VEM data processing workflow is highly complex and typically involves the following stages:

1. **2D Image Stitching**  
2. **3D Slice Alignment / Registration**  
3. **Slice Damage Restoration & Axial Interpolation (Inpainting / Axial Flow)**  
4. **Isotropic 3D Reconstruction**  
5. **3D Structural Segmentation**

This project aims to develop an AI-driven system that covers the *entire* VEM processing pipeline, enabling researchers to efficiently complete the full workflow from **raw slices → 3D volume reconstruction → biological analysis**.

---

## 🎯 Goals and Objectives

Despite substantial progress in VEM methodologies, several key challenges remain unresolved:

1. Accurately matching image features within complex biological structures while modeling both global rigidity and local elastic deformation for precise stitching.  
2. Preserving Z-axis structural coherence, restoring damaged slices faithfully, and distinguishing natural biological deformation from nonlinear imaging artifacts.  
3. Achieving isotropic 3D reconstruction at arbitrary resolutions through implicit neural representations.  
4. Leveraging minimal prompt information with large pre-trained models to enable accurate segmentation of diverse biological structures.

To address these challenges, the following objectives are defined:

### 🔹 Objective 1: High-Precision Image Stitching
Develop a stitching framework capable of handling both global rigid alignment and local elastic deformation, enabling accurate feature matching and producing seamless, high-resolution panoramic slices.

### 🔹 Objective 2: Accurate 3D Alignment
Design a 3D alignment method that incorporates slice-damage repair using axial structural continuity. Axial optical flow will capture Z-axis structural changes, while learned deformation fields correct nonlinear distortions to restore natural biological geometry.

### 🔹 Objective 3: Self-Supervised 3D Reconstruction
Introduce a self-supervised reconstruction approach based on implicit neural representations to generate high-fidelity, isotropic 3D volumes at multiple resolutions using continuous positional encoding and artifact-free interpolation.

### 🔹 Objective 4: Efficient 3D Structure Segmentation
Develop a large pre-trained model for VEM segmentation, enabling zero-shot transfer and interactive prompt-based refinement to accurately segment diverse organelles and complex cellular structures with minimal manual annotation.

**In summary**, these objectives aim to overcome key barriers in VEM processing, advancing high-resolution 3D reconstruction and unlocking deeper insights into complex biological systems for health and life science research.

---

## 📚 Existing Methods & Publications

Below lists our existing research contributions corresponding to each step of the VEM pipeline, including **paper links** and **open-source code (if available)**.

---

### 🔹 1. 2D Image Stitching  
**vEMstitch: Fully Automatic Image Stitching for VEM**  
- 📄 Paper (GigaScience 2024):  
  https://doi.org/10.1093/gigascience/giae076  
- 💻 Code:  
  https://github.com/DeepImagingLab/vEMstitch

---

### 🔹 2. 3D Slice Alignment / Registration

#### (a) Gaussian Filter–Based 3D Registration  
- 📄 Paper (AAAI 2025):  
  Zhenbang Zhang, Hongjia Li, Zhiqiang Xu, Wenjia Meng*, Renmin Han*.  
  *A Gaussian filter-based 3D registration method for serial section EM.*  
- 💻 Code: *(to be released)*

#### (b) Neural ODE–based Self-Supervised 3D Registration  
- 📄 Paper (NeurIPS 2025):  
  Zhenbang Zhang, Jingtong Feng, Hongjia Li, Haythem El-Messiry, Zhiqiang Xu*, Renmin Han*.  
  *Unsupervised Trajectory Optimization for 3D Registration in Serial Section EM using Neural ODEs.*  
- 💻 Code: *(to be released)*

---

### 🔹 3. Slice Damage Restoration / Axial Inpainting  
- 📄 Paper (ACM Multimedia 2024):  
  Yiran Cheng, Bintao He, Fa Zhang, Renmin Han*.  
  *Serial section microscopy image inpainting guided by axial optical flow.*  
  https://doi.org/10.1145/XXXX.XXXX  *(replace with final DOI when available)*  
- 💻 Code: *(to be released)*

---

### 🔹 4. Implicit Neural Representation (INR) for 3D Reconstruction  
- Method integrated in this project (self-supervised, anisotropy-aware).  
- 📄 Related works:  
  (Provide once you have the official preprint / publication)  
- 💻 Code: *(to be released)*

---

### 🔹 5. 3D Structural Segmentation with Large Models  
- Large pretrained model + promptable segmentation  
- 📄 Related research from team (examples):  
  - Deep representation learning, contrastive learning, segmentation foundations  
  - (You may insert specific papers later if desired)
- 💻 Code: *(to be released)*
