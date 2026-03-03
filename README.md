# Modeling Elastoviscoplastic Materials Using Physics-Informed Neural Networks

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This repository contains the official PyTorch data and code implementation for the paper: **"Modeling Elastoviscoplastic Materials Using Physics-Informed Neural Networks"** by Babak Valipour Goodarzi and Reza Foudazi (The University of Oklahoma).

## 📄 About the Paper
Elastoviscoplastic (EVP) materials pose significant challenges for predictive modeling, especially under large amplitude oscillatory shear (LAOS) conditions due to their nonlinear rheological behavior. While various models have been proposed to describe yielding and viscoelastic transitions, their application to experimental data remains limited due to computational complexity, poor generalizability, and difficulty in fitting noisy data. 

This work re-evaluates rheological modeling of EVP materials by using a Physics-Informed Neural Network (PINN) approach that embeds a modified Saramito model into the training framework. By directly fitting time-dependent stress data on typical EVP materials, this method circumvents the need for gradient estimation from noisy measurements and offers a data-efficient, differentiable, and generalizable alternative to conventional fitting methods. A strain-softening formulation is introduced to reflect the decreasing elasticity and viscosity at higher strain amplitudes.

## 🗂️ Repository Structure

### Data (`/data`)
This folder contains the experimental data of the attractive nanoemulsion with 40% volume fraction of PDMS oil dispersed in water. Various strain amplitudes at the fixed frequency of 10 rad/s

### Notebooks
The root directory contains Jupyter Notebooks that walk through the training and evaluation of the models:
* `Classic_Saramito_Synthetic.ipynb`: Validates the PINN framework using synthetic data.
* `Classic_Saramito_Experimental.ipynb`: Applies the classic model to experimental data.
* `Updated_Saramito_Decaying_Dashpot.ipynb`: Model incorporating a decaying dashpot formulation.
* `Updated_Saramito_Decaying_Dashpot_Spring.ipynb`: Model incorporating both decaying dashpot and spring elements.

- This research was supported by the School of Sustainable Chemical, Biological and Materials Engineering at the University of Oklahoma.

- The authors acknowledge the use of AI language models, specifically OpenAI's ChatGPT and Google's Gemini, which provided assistance in drafting and troubleshooting portions of the Python/PyTorch code in this repository.

## 🖋️ Citation
If you utilize this code or data in your research, please cite our upcoming paper. 

*(Note: Citation details will be updated upon final publication)*

```bibtex
@article{Goodarzi_Foudazi_202X,
  title={Modeling Elastoviscoplastic Materials Using Physics-Informed Neural Networks},
  author={Goodarzi, Babak Valipour and Foudazi, Reza},
  journal={Under Review},
  year={202X}
}

## ⚙️ Installation & Usage
To run the code locally, we recommend creating a virtual environment and installing the dependencies:

```bash
# Clone the repository
git clone [https://github.com/YourUsername/PINN_EVP_Rheology.git](https://github.com/YourUsername/PINN_EVP_Rheology.git)
cd PINN_EVP_Rheology

# Install requirements

pip install -r requirements.txt
