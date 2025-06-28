# CIFAR-10-Model-Comparison


# 🎯 Objective

Compare the performance and efficiency of four deep learning architectures — **AlexNet**, **VGG16**, **ResNeXt50**, and **ViT** — on a custom CIFAR-10 dataset using PyTorch.


# 📦 Dataset

**Source:** Custom Kaggle CIFAR-10 Dataset  
- Format: `.7z` compressed folders  
- `train.7z` — Training images  
- `test.7z` — Testing images  
- `trainLabels.csv` — Labels  
- 10 classes (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck)



## ⚙️ Preprocessing Steps

- Extract `.7z` files using `py7zr`
- Resize all images to **224×224**
- Normalize pixel values to range `[0, 1]`
- Train/Validation/Test split: **70% / 20% / 10%**


## 🧠 Models Used

| Model      | Type        | Key Feature                      |
|------------|-------------|----------------------------------|
| AlexNet    | CNN         | Shallow & fast                   |
| VGG16      | CNN         | Deep with large FC layers        |
| ResNeXt50  | CNN         | Grouped convolutions (efficient) |
| ViT Base   | Transformer | Attention-based vision model     |

All models were pre-trained on ImageNet and fine-tuned on CIFAR-10.

---

## 📈 Evaluation Metrics

- Accuracy  
- Precision, Recall, F1-Score (per class)  
- Confusion Matrix  
- Training Time  
- Inference Time  
- Model Parameters (Millions)



## 📊 Results Summary

| Model     | Accuracy | Params (M) | Train Time | Inference Time |
|-----------|----------|------------|------------|----------------|
| AlexNet   | ~77%     | 61.1       | Fast       | Very Fast      |
| VGG16     | ~82%     | 138.4      | Slow       | Moderate       |
| ResNeXt50 | ~85%     | 22.9       | Moderate   | Fast           |
| ViT Base  | ~88%     | 86.4       | Moderate   | Moderate       |


---

## 📌 Key Findings

- **ViT** performs best in accuracy but is slower in inference.
- **ResNeXt50** offers the best trade-off between accuracy and speed.
- **VGG16** is large and slower, despite good accuracy.
- **AlexNet** is fastest but underperforms on complex patterns.

---

## 📚 SDG Alignment

- **SDG 4** – Quality Education  
- **SDG 9** – Industry, Innovation, and Infrastructure  
# Output: [kaggle kernels output syedalihasnat/ciraf-10 -p /path/to/dest]
[https://www.kaggle.com/code/syedalihasnat/ciraf-10]
---

## 👨‍💻 Author

- **Ali Hasnat**
- BE SE — Iqra University

> Contributions welcome! For issues or suggestions, open an issue or pull request.



