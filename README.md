# MLSec-Project:
# Adversarial Robustness: CIFAR-10 vs CIFAR-10.1
## Team
KADRI Ikram _ 70/90/00692

HOUACINE Yousra _ 70/90/00693

AISSANI Rafik Yudas _ 70/30/00694

# Overview
This project evaluates the generalization of adversarial robustness. We compared State-of-the-Art (SOTA) models from RobustBench to see if their performance holds up on CIFAR-10.1, a newer test set designed to minimize distribution shift issues found in the original CIFAR-10.
We wanted to verify if high robustness scores on the leaderboard are due to "overfitting" to the specific pixels of CIFAR-10 or if they represent true security.
# Technical SetupModels:
We selected three models with different architectures and training dates:
Bartoldson2024Adversarial_WRN-94-16 (Current Top 1).

Rebuffi2021Fixing_70_16_cutmix_extra (Stable 2021 baseline).

Zhang2019Theoretically (The TRADES classic).
## Attack:
AutoAttack ($L_{\infty}$ norm, $\epsilon = 8/255$).
## Data: 
We used 200 balanced images (20 per class) from both CIFAR-10 and CIFAR-10.1.
