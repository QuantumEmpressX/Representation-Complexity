# Representation-Complexity
This repository contains the source code for the spectral analysis metrics proposed in the research paper: "Representation Compression and Generalization in Neural Networks: A Spectral-Information Framework".
Overview
This project provides tools to measure the complexity of internal representations in deep neural networks. By calculating the Effective Spectral Dimension (D_{eff}) and Representation Entropy (H) of hidden-layer activations, this framework allows researchers to quantify how neural networks "compress" information during the training process.
Key Features
Spectral Analysis: Compute the eigenvalue spectrum of activation covariance matrices.
Complexity Metrics: Calculate intrinsic representation dimensionality and information-theoretic entropy.
PyTorch Integration: Designed to be easily inserted into existing training loops.
Usage
You can import the compute_metrics function to analyze your model's hidden layers:



import torch
from metrics import compute_metrics

# Assuming 'activations' is a tensor of shape (n_samples, n_features)
d_eff, entropy = compute_metrics(activations)

print(f"Effective Spectral Dimension: {d_eff}")
print(f"Representation Entropy: {entropy}")


Requirements
torch (PyTorch)
numpy
Citation
If you use this code in your research, please cite our paper:
(Insert your paper title here once published on arXiv)
How to use this in GitHub:
On your repository page, click "Add file" > "Create new file".
Name the file exactly README.md (all caps, with a dot).
Paste the text above into the large box.
Scroll down and click the green "Commit changes" button.




