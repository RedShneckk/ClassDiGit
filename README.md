# ClassDiGit — MNIST Classifier (TinyGrad + WebGPU)

An interactive web application that recognizes hand-drawn digits (0-9) using two neural network architectures trained in **TinyGrad**, running locally in your browser via **WebGPU**.

---

**Live Demo Link:** [ClassDiGit (GitHub Pages)](https://redshneckk.github.io/ClassDiGit/)


---

**ClassDiGit** demonstrates end-to-end machine learning from model training to in-browser inference.  
Two models (a **Multilayer Perceptron (MLP)** and a **Convolutional Neural Network (ConvNet)**) are trained on the MNIST dataset using **TinyGrad**.  
The exported models are then integrated into a **WebGPU-powered web interface**, allowing users to draw digits and get instant predictions directly on their device.

---

## Features
- Draw digits on a responsive 360×360 canvas.  
- Switch between **MLP** and **ConvNet** inference modes.  
- Real-time prediction with softmax probability bars.  
- Eraser and clear-canvas tools.  
- Instant inference using the GPU via WebGPU.  
- Clean UI built with TailwindCSS.  
- WebGPU availability check and fallback notice.

---

## Model Summary

| Model          | Accuracy (Test) |  
| `mnist_mlp`    | 96.7 %          | 
| `mnist_convnet`| 99.1 %          | 

## Full training details and hyperparameter 
available in [`HYPERPARAMETERS.md`](./HYPERPARAMETERS.md).

---

## Setup / Local Run

### Clone or download this repository
```bash
git clone https://github.com/<your-github-username>/ClassDiGit.git
cd ClassDiGit
