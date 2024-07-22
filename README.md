# HybridGrasp
code for ‘HybridGrasp:A vision-language-action Modeling for Task-Oriented Grasping’，the code is coming soon.
## Method
![zjw2](https://github.com/user-attachments/assets/891e4445-9d34-4cac-947d-942a408bd25c)
Language instructions are utilized to obtain object category descriptions, task descriptions, and grasping descriptions.These descriptions and language instructions are input into a pre-trained text enpdfcoder to generate text features. Simultaneously, point cloud data is fed into both a point cloud encoder and a pre-trained FGC-GraspNet module, producing point cloud features and a set of grasping poses encoded as spatial features. The grasping poses are then processed by an action encoder to generate action features. These features are integrated using a cross-attention module, where action features serve as queries, point cloud features as keys, and language features as values, resulting in the generation of cross-attention features. Finally, the policy module takes the cross-attention features as input to output evaluation results for all actions.
## Results
![result2](https://github.com/user-attachments/assets/811dcb15-d4f6-424e-ad74-6f1cc6c8b4c5)
![result1](https://github.com/user-attachments/assets/3633db3e-2828-4896-aee8-b57f25c597fc)
![zjw3](https://github.com/user-attachments/assets/0670b395-e665-4647-b283-84bde8e0ea0f)
## Real robot experiment
![zjw4](https://github.com/user-attachments/assets/ec6091f7-aec8-421b-b1f2-097096882a66)
