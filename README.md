# ZAF043 Auto Pilot 
## Overview

Using deep learning techniques, an autopilot system for autonomous driving was developed based on the Carla simulator. The system is capable of driving a car automatically for up to 100 meters. Image data captured during car driving serves as input, and a variational autoencoder is employed for data reconstruction. The deep learning model is trained using this reconstructed data and leverages the PPO algorithm for optimization. This combination of techniques enables the autopilot system to understand and interpret visual input from the car's perspective, leading to autonomous driving capabilities in the simulated environment. It's important to note that while this achievement is significant, the development of a comprehensive and safe autonomous driving system involves additional challenges, such as perception, planning, control, and real-world deployment considerations.

## Methodology
- Data Collection: Collect image data of car driving from the Carla simulator. This data captures the visual input perceived by the car 
  during different driving scenarios.

- Variational Autoencoder (VAE) Reconstruction: Apply a variational autoencoder to reconstruct the image data. A variational autoencoder is a type of neural network that can learn an efficient representation of data and reconstruct it. By leveraging the VAE, the image data is processed and reconstructed, potentially enhancing the features and reducing noise.

- Dataset Preparation: Prepare the dataset by combining the original image data with the reconstructed image data from the VAE. This creates a training dataset that includes both the original images and the corresponding reconstructed images.

- Deep Learning Model: Design a deep learning model, likely a convolutional neural network (CNN), to process and interpret the visual input. The model architecture is tailored to handle the specific task of autonomous driving, such as object detection, lane following, or obstacle avoidance.

- PPO Training: Utilize the Proximal Policy Optimization (PPO) algorithm to train the deep learning model. PPO is a reinforcement learning algorithm that optimizes policies through iterative updates. During training, the model interacts with the simulated environment, receives rewards or penalties based on its actions, and adjusts its policy accordingly to maximize performance.

- Training and Evaluation: Train the deep learning model on the combined dataset using the PPO algorithm. Evaluate the performance of the model by testing it in various driving scenarios within the Carla simulator, measuring metrics such as accuracy, safety, and efficiency.

- Iterative Refinement: Iterate and refine the model and training process based on evaluation results. This may involve adjusting hyperparameters, modifying the model architecture, or incorporating additional techniques to enhance performance and address any shortcomings.
## AI Application
- NLP

## Business Segments
- Lifestyle & Social Media, Media & Publishing
- Business & Private Sector

## Use Case Development can be found [here](https://docs.google.com/document/d/1V070_FZStj2Sp_UYRbYDVAHzKyz9P5wBXHR2JNOzw6M/edit?usp=sharing).
