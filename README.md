# 🔍 Variational Autoencoder with GMM Clustering on MNIST (Digits 1, 4, 8)

This project demonstrates an end-to-end implementation of a **Variational Autoencoder (VAE)** coupled with **Gaussian Mixture Model (GMM)** clustering to learn and visualize the latent space of MNIST digits **1, 4, and 8**.

It includes training, latent space visualization, digit reconstruction, and unsupervised digit classification using GMM.

---

## 🚀 Pipeline

✅ Trains a Variational Autoencoder (VAE) on digits {1, 4, 8}  
✅ Learns a 2D latent representation of digits  
✅ Visualizes reconstructed images and the latent manifold  
✅ Applies GMM (from scratch and via `scikit-learn`) for clustering  
✅ Maps GMM clusters to digit labels using validation data  
✅ Generates predictions and saves results to CSV  

---

## 🧠 Model Architecture
### 🔸 Variational Autoencoder (VAE)
- Encoder: 784 → 256 → 128 → latent space (2D)
- Decoder: latent space → 128 → 256 → 784
- Latent dimension: 2
- Loss: Binary Cross Entropy + KL Divergence

### 🔸 Gaussian Mixture Model (GMM)
- Applied in 2D latent space
- 3 components (one per digit: 1, 4, 8)
- Trained via scikit-learn and custom EM implementation

--- 

## 📦 Dependencies

Install the required libraries using pip:

```bash
pip install numpy pandas matplotlib seaborn torch scikit-learn
```
