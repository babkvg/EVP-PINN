# Modeling Elastoviscoplastic Materials Using Physics-Informed Neural Networks

This repository contains the official PyTorch implementation for the paper: **"Modeling Elastoviscoplastic Materials Using Physics-Informed Neural Networks"** by Babak Valipour Goodarzi and Reza Foudazi.

## Overview
This repository provides a Physics-Informed Neural Network (PINN) framework that embeds a modified Saramito model to directly fit time-dependent stress data for Elastoviscoplastic (EVP) materials under large amplitude oscillatory shear (LAOS). 

## Files
* `Classic_Saramito_Synthetic.ipynb`: Validates the PINN framework using synthetic data.
* `Classic_Saramito_Experimental.ipynb`: Applies the classic model to experimental data.
* `Updated_Saramito_Decaying_Dashpot.ipynb`: Model incorporating a decaying dashpot.
* `Updated_Saramito_Decaying_Dashpot_Spring.ipynb`: Model incorporating both decaying dashpot and spring elements.

## Installation
```bash
pip install -r requirements.txt