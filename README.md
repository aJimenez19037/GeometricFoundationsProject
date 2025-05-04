# GeometricFoundationsProject

## Purpose
Robust autonomous driving under uncertain conditions is a very challenging sequential decision problem requiring precise estimation of the vehicle's state as well as safe prediction of other vehicles' behaviors. Given that there could be catastrophic consequences of poor decisions, autonomous driving systems not only need to maximize their expected performance, but also behave robustly in worst-case scenarios.

## Contribution

We aim to expand upon the baseline approaches mentioned within other similar papers, especially with regard to uncertainty within sensor errors. We propose to improve the robustness and decision quality of autonomous driving policies by explicitly modeling sensor noise using Normalizing Flow (NF) models, which are capable of accurately capturing multi-modal intricate distributions that are typical of real-world sensor noise. This allows for probabilistic sensor measurement modeling, which integrates naturally with the reinforcement learning procedure. Thus, the policy created is more informed and robust, allowing it to effectively manage the uncertainties of monitoring vehicle states and predicting nearby behaviors.

By incorporating NF-based uncertainty modeling in combination with a baseline approach of using a Soft Actor-Critic for Discrete Action Settings (SAC-Discrete) algorithm with a Motion Predictive Safety Controller (MPSC), our approach is specifically targeted to tackle improvements for the scenario of inaccurate vehicle state tracking. Not only does this incorporation facilitate greater policy robustness, but also helps with improved real-time response and safety overall, which we aimed to validate with our experiments.

## Files
CS_378_Final_report_Phase_1.pdf - Report for phase 1 of the project

CS_378_Final_report_Phase_2.pdf - Report for phase 2 of the project

CS_378_Final_Project.ipynb contains the jupyter notebook for phase 1 and phase 2 of the project.

NF_DATA.zip contains data collected from 9000 episodes utilized to create normalizing flow models. Combined, easy, medium, and hard environment data files.

NF_model.zip contains normalizing flow models

agents_hard.zip contains 5 different agents: SAC (true), SAC + MPSC (true), SAC (noise), SAC + MPSC (noise), SAC + MPSC + NF (true)

## Google colab
Google colab utilized for the developement of the project: https://colab.research.google.com/drive/16fQsgVxc6T2F11QZsxdvuIC24ZIo6IcK?usp=sharing
