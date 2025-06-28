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

| Model      | Parameters | Train Time (s) | Inference Time (ms) | Accuracy  |
|------------|------------|----------------|----------------------|-----------|
| AlexNet    | ~61M       | ~68            | ~2.3                 | ~89%      |
| VGG16      | ~134M      | ~96            | ~3.5                 | ~92%      |
| ResNeXt50  | ~25M       | ~82            | ~2.9                 | ~95%      |
| ViT Base   | ~86M       | ~71            | ~5.7                 | ~95%      |


---

## 📌 Key Observations
ViT and ResNeXt50 outperformed the others in accuracy.

ResNeXt provided the best trade-off between speed and performance.

AlexNet, while outdated, still performed decently on CIFAR-10.

Inference time and model size vary significantly — critical for deployment.


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



