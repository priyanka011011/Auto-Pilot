# ZAF043 Auto Pilot 
## Overview

Using deep learning techniques, an autopilot system for autonomous driving was developed based on the Carla simulator. The system is capable of driving a car automatically for up to 100 meters. Image data captured during car driving serves as input, and a variational autoencoder is employed for data reconstruction. The deep learning model is trained using this reconstructed data and leverages the PPO algorithm for optimization. This combination of techniques enables the autopilot system to understand and interpret visual input from the car's perspective, leading to autonomous driving capabilities in the simulated environment. It's important to note that while this achievement is significant, the development of a comprehensive and safe autonomous driving system involves additional challenges, such as perception, planning, control, and real-world deployment considerations.

![Screen-Shot-2020-03-23-at-5 48 27-AM-e1584968282707](https://github.com/priyanka011011/Auto-Pilot/assets/63203112/baef228c-9ab2-4c86-b735-62690f83b48b)

## Methodology
- [Data Collection](https://www.simplilearn.com/what-is-data-collection-article): Collect image data of car driving from the Carla simulator. This data captures the visual input perceived by the car 
  during different driving scenarios.

- [Variational Autoencoder (VAE) Reconstruction](http://dm.snu.ac.kr/static/docs/TR/SNUDM-TR-2015-03.pdf): Apply a variational autoencoder to reconstruct the image data. A variational autoencoder is a type of neural network that can learn an efficient representation of data and reconstruct it. By leveraging the VAE, the image data is processed and reconstructed, potentially enhancing the features and reducing noise.

- [Dataset Preparation](https://blog.jetbrains.com/datalore/2022/11/08/how-to-prepare-your-dataset-for-machine-learning-and-analysis/): Prepare the dataset by combining the original image data with the reconstructed image data from the VAE. This creates a training dataset that includes both the original images and the corresponding reconstructed images.

- [Deep Learning Model](https://www.simplilearn.com/tutorials/deep-learning-tutorial/deep-learning-algorithm): Design a deep learning model, likely a convolutional neural network (CNN), to process and interpret the visual input. The model architecture is tailored to handle the specific task of autonomous driving, such as object detection, lane following, or obstacle avoidance.

- [PPO Training](https://openai.com/research/openai-baselines-ppo): Utilize the Proximal Policy Optimization (PPO) algorithm to train the deep learning model. PPO is a reinforcement learning algorithm that optimizes policies through iterative updates. During training, the model interacts with the simulated environment, receives rewards or penalties based on its actions, and adjusts its policy accordingly to maximize performance.

- [Training and Evaluation](https://www.researchgate.net/publication/369776800_Deep_Reinforcement_Learning_for_Vision-Based_Navigation_of_UAVs_in_Avoiding_Stationary_and_Mobile_Obstacles): Train the deep learning model on the combined dataset using the PPO algorithm. Evaluate the performance of the model by testing it in various driving scenarios within the Carla simulator, measuring metrics such as accuracy, safety, and efficiency.

- [Iterative Refinement](https://blogs.mathworks.com/cleve/2015/02/16/iterative-refinement-for-solutions-to-linear-systems/): Iterate and refine the model and training process based on evaluation results. This may involve adjusting hyperparameters, modifying the model architecture, or incorporating additional techniques to enhance performance and address any shortcomings.


## AI Application
- [Object Detection and Recognition]: AI algorithms, such as convolutional neural networks (CNNs), are used to detect and recognize objects in the environment surrounding the vehicle. This enables the autopilot system to identify and track vehicles, pedestrians, traffic signs, and other relevant objects.

- [Path Planning and Control]: AI algorithms are employed to plan and execute the vehicle's trajectory, ensuring safe and efficient navigation. Reinforcement learning and model predictive control techniques can be utilized to optimize path planning and control decisions based on real-time sensor inputs.

- [Sensor Fusion]: Autonomous vehicles often use multiple sensors, such as cameras, lidar, radar, and GPS, to perceive the environment. AI algorithms are applied to fuse and integrate information from these sensors, enabling a more comprehensive understanding of the surroundings.

- [Localization and Mapping]: AI algorithms, including simultaneous localization and mapping (SLAM), help the autopilot system accurately determine the vehicle's position and create a detailed map of the environment. This information is crucial for navigation and situational awareness.

- [Decision-Making and Risk Assessment]: AI algorithms play a critical role in decision-making by analyzing sensor data and predicting potential hazards or obstacles. These algorithms consider various factors, such as traffic conditions, speed limits, and the behavior of other vehicles, to make informed decisions while minimizing risks.

- [Adaptive Learning and Continuous Improvement]: Autopilot systems can employ AI techniques to continuously learn and improve their performance. By analyzing real-time driving data and user feedback, the system can adapt its behavior, optimize its decision-making algorithms, and enhance overall driving capabilities.

- [Safety and Emergency Handling]: AI algorithms are utilized to identify critical situations and take appropriate actions, such as emergency braking or collision avoidance, to ensure the safety of the vehicle and its occupants.

## Business Segments
Autopilot systems and autonomous driving technologies have the potential to impact various business segments. Here are some key business segments that can benefit from the development and implementation of autopilot systems:

1. [Automotive Manufacturers]: Traditional automotive manufacturers can incorporate autopilot features into their vehicles, offering advanced driver-assistance systems [ADAS](https://www.aptiv.com/en/insights/article/what-is-adas#:~:text=Advanced%20driver%2Dassistance%20systems%20(ADAS,active%20safety%E2%80%9D%20are%20used%20interchangeably.) and autonomous driving capabilities. This allows them to compete in the evolving automotive market and cater to customers seeking enhanced safety and convenience.

2. [Ride-Hailing and Ride-Sharing Services]: Companies operating in the ride-hailing and ride-sharing industry can leverage autopilot systems to offer self-driving vehicle services. This could reduce operating costs by eliminating the need for human drivers and provide an improved customer experience with efficient and safe transportation.

3. [Logistics and Delivery Services]: Autopilot systems can revolutionize the logistics and delivery industry by enabling autonomous vehicles for shipping, last-mile delivery, and warehouse operations. This can lead to increased efficiency, reduced costs, and improved logistics management.

4. [Public Transportation]: Autonomous buses or shuttles equipped with autopilot systems can transform public transportation by offering efficient and reliable services. This can help reduce traffic congestion, enhance passenger safety, and improve the overall quality of public transportation systems.

5. [Agriculture]: Autopilot systems can be integrated into agricultural machinery, such as tractors and harvesters, to automate farming operations. This enables precision farming techniques, reduces labor costs, optimizes resource utilization, and improves crop yields.

6. [Insurance]: The adoption of autopilot systems can influence the insurance industry. Insurers may need to adapt their policies and pricing models to account for the shifting risk landscape associated with autonomous vehicles.

7. [Infrastructure and Smart Cities]: Autopilot systems and autonomous driving technologies require supportive infrastructure, such as smart traffic management systems and advanced communication networks. Companies specializing in infrastructure development and smart city solutions can benefit from the demand for these technologies.

8. [Data and Analytics]: With autopilot systems generating vast amounts of data, businesses focused on data analytics and artificial intelligence can provide services for processing, analyzing, and deriving insights from the collected data. This can assist in improving the performance and safety of autonomous driving systems.

9. [Sensor and Technology Providers]: Companies involved in sensor technology, lidar, radar, and camera systems can supply the necessary hardware and technology components for autopilot systems. Advancements in these technologies will drive innovation and competitiveness in the market.

10. [Software and Algorithm Development]: Autopilot systems heavily rely on software and algorithms for perception, decision-making, and control. Businesses specializing in software development, deep learning, and artificial intelligence algorithms can contribute to the development and improvement of autonomous driving technologies.

These are just a few examples of the business segments that can be impacted by the adoption and implementation of autopilot systems and autonomous driving technologies. As the technology continues to evolve, new opportunities and business models are likely to emerge in various sectors.

## Objective

The objective of developing an autopilot system for autonomous driving can vary based on the specific goals and requirements of the project. 

1. [Enhancing Safety]: One of the primary objectives of an autopilot system is to improve road safety by reducing the number of accidents caused by human error. The system aims to minimize the risk of collisions, provide reliable obstacle detection and avoidance, and respond effectively to potential hazards on the road.

2. [Increasing Efficiency and Convenience]: Autopilot systems aim to optimize driving efficiency by reducing traffic congestion, minimizing fuel consumption, and improving overall transportation efficiency. They also offer the convenience of hands-free driving and the ability to focus on other tasks during the journey.

3. [Enabling Mobility for All]: Autonomous driving technology has the potential to provide mobility solutions for individuals who are unable to drive, such as the elderly or people with disabilities. The objective is to create an inclusive transportation system that enhances mobility and independence for all individuals.

4. [Reducing Environmental Impact]: Autopilot systems can contribute to reducing the environmental impact of transportation by promoting efficient driving patterns, optimizing routes, and facilitating the adoption of electric and alternative fuel vehicles. The objective is to support sustainable transportation practices and mitigate the effects of climate change.

5. [Advancing Technology and Innovation]: The development of autopilot systems aims to push the boundaries of technology and drive innovation in the automotive industry. It involves the application of cutting-edge technologies, such as artificial intelligence, machine learning, and sensor fusion, to create advanced autonomous driving capabilities.

6. [Improving User Experience]: Autopilot systems strive to provide a seamless and enjoyable driving experience for users. The objective is to create intuitive interfaces, user-friendly controls, and comfortable travel conditions that enhance user satisfaction and acceptance of autonomous driving technology.

7. [Facilitating Business Opportunities]: The objective of developing autopilot systems extends to creating new business opportunities in sectors such as ride-hailing, logistics, and mobility services. Autonomous vehicles can unlock innovative business models and revenue streams, providing economic benefits for companies and entrepreneurs.

## Model

The [Proximal Policy Optimization (PPO)](https://spinningup.openai.com/en/latest/algorithms/ppo.html) algorithm is a reinforcement learning algorithm that is widely used in training autonomous driving models and other applications. It is designed to optimize policies in environments where an agent such as the [autopilot system](https://www.flypgs.com/en/travel-glossary/autopilot#:~:text=An%20autopilot%20is%20a%20software,of%20the%20aircraft%20(heading) learns to make sequential decisions to maximize its cumulative rewards.

![High-level-diagram-of-the-proximal-policy-optimization-algorithm](https://github.com/priyanka011011/Auto-Pilot/assets/63203112/e34bfc9f-822d-403d-a3b6-e754d29f1615)

## Dataset

This dataset encompasses about 60 individual drives of a 2020 Tesla Model 3 with Autopilot in its relevant operational domain covering more than 1,000 miles. The majority of the data was collected during highway and suburban driving. Information collected includes vehicle CAN data as well as Lidar and camera data from a vehicle mounted sensor array. Vehicle CAN data and information on traffic surrounding the Ego-vehicle derived from the sensor array are postprocessed and merged to provide one combined CVS data file per drive. 

- [Dataset Download](https://www.osti.gov/dataexplorer/biblio/dataset/1922211)

![compositor](https://github.com/priyanka011011/Auto-Pilot/assets/63203112/8d13082b-63ab-43ee-bdde-68186f3580e8)

## Papers
- Deep-Learning-Based Neural Network Training for State Estimation Enhancement: Application to Attitude Estimation
     - [Paper](https://ieeexplore.ieee.org/abstract/document/8643440?casa_token=7UEXpLIND5gAAAAA:WZSGDuc1fvWuk2sfwE4D8QsyhK47Xf8SXfJOpnwDpMITY65MFRGBAK4T5MKdzgi7SQuVDKAPiw)
     - [BitTex](https://scholar.googleusercontent.com/scholar.bib?q=info:BnQbP7t8KYwJ:scholar.google.com/&output=citation&scisdr=Cm13JnzVEMW_o-NUyp0:AGlGAw8AAAAAZHxS0p0c9vS0vYXoZjkno0450f8&scisig=AGlGAw8AAAAAZHxS0pUheaeAKXK6Wip-Heq-7uk&scisf=4&ct=citation&cd=-1&hl=en)
- Visual Autopilot Decision System Based on Deep Learning
     - [Paper](https://link.springer.com/chapter/10.1007/978-981-16-3391-1_38)
     - [BitTex](https://scholar.googleusercontent.com/scholar.bib?q=info:L7u4tiPQ77kJ:scholar.google.com/&output=citation&scisdr=Cm13JnzVEMW_o-NVb-8:AGlGAw8AAAAAZHxTd-_lVsK6sZX0M3WXD1qvVrU&scisig=AGlGAw8AAAAAZHxTd-NEyWrfouu6FDTU4By1GyY&scisf=4&ct=citation&cd=-1&hl=en)
 - Smart Autopilot Drone System for Surface Surveillance and Anomaly Detection via Customizable Deep Neural Network
      - [Paper](https://onepetro.org/IPTCONF/proceedings-abstract/20IPTC/2-20IPTC/154708)
      - [BitTex](https://scholar.googleusercontent.com/scholar.bib?q=info:7GertA_hWDgJ:scholar.google.com/&output=citation&scisdr=Cm13JnzVEMW_o-NVziM:AGlGAw8AAAAAZHxT1iMeQuLb6IxLKqht1fou6gI&scisig=AGlGAw8AAAAAZHxT1tMUhStBYpBj0f8K0kerOJI&scisf=4&ct=citation&cd=-1&hl=en)
 
## Team
- Sanjeeb Tiwary 
   - [sanjeebtiwary](https://github.com/sanjeebtiwary)
