# vision-similarity-detection

## 🧠📸 Project Overview
This project explores two core areas of computer vision:  
1. **Image Similarity Analysis** → comparing visual similarity between images using statistical and perceptual metrics.  
2. **Object Detection** → identifying and labeling objects in images using a deep learning model.  

The work was developed as part of an academic assignment to demonstrate practical applications of similarity measures and deep learning–based detection.

---

## 📂 Repository Structure
- **Homework6_Combined_Image_Similarity_Object_Detection.ipynb** → Jupyter notebook with full implementation, visualizations, and results  
- **Homework6_Report.pdf** → Written report outlining methods, models, and findings  
- **Bright_Tree.png, Dark_Tree.png** → Input images for similarity evaluation  
- **Kitchen.jpg, StreetView.jpg, Zebra.jpg** → Test images for object detection  

---

## 🧪 Tasks & Methods

### 🔹 Part A: Image Similarity
- **Goal:** Compare `Bright_Tree` vs `Dark_Tree`  
- **Metrics Used:**  
  - *MSE* (Mean Squared Error)  
  - *PSNR* (Peak Signal-to-Noise Ratio)  
  - *SSIM* (Structural Similarity Index)  
- **Techniques Applied:**  
  - Histogram matching to reduce brightness differences  
  - Grayscale conversion for SSIM analysis  
  - Pre- and post-enhancement evaluation  

---

### 🔹 Part B: Object Detection
- **Goal:** Detect objects in `Kitchen.jpg`, `StreetView.jpg`, and `Zebra.jpg`  
- **Model:** `fasterrcnn_resnet50_fpn` (PyTorch pretrained)  
- **Threshold:** Confidence ≥ 0.7  
- **Output:** Bounding boxes + class labels  

---

## 📊 Results

### Image Similarity
| Metric | Original | After Histogram Matching |
|--------|----------|--------------------------|
| **MSE** | 0.0209 | 0.0131 |
| **PSNR** | 16.81 dB | 18.83 dB |
| **SSIM** | 0.7371 | 0.7720 |

➡ Histogram matching significantly improved similarity scores.

### Object Detection
| Image       | Objects Detected (≥ 0.7) |
|-------------|--------------------------|
| **Kitchen** | bottle, cup, potted plant, dining table, chair |
| **StreetView** | car, person, bus |
| **Zebra** | zebra ×2 (100% confidence) |

---

## 🛠️ Tools & Libraries
- Python 3.x  
- NumPy, OpenCV, scikit-image  
- Matplotlib  
- PyTorch & torchvision  

---

## 📄 License
This repository is for **academic use only**.  

⭐ If you found this useful, consider forking or starring the repo!
