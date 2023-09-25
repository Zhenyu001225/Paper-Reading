Title: [019][Robustness][Theoretically Analysis] Parametric Noise Injection: Trainable Randomness to Improve Deep Neural Network Robustness against Adversarial Attack
Authors:  Zhezhi He, Adnan Siraj Rakin and Deliang Fan
Affiliations: Dept. of Electrical and Computer Engineering, University of Central Florida, Orlando
Venue: CVPR 2019
Link: https://openaccess.thecvf.com/content_CVPR_2019/html/He_Parametric_Noise_Injection_Trainable_Randomness_to_Improve_Deep_Neural_Network_CVPR_2019_paper.html
Code Link: https:// github.com/elliothe/CVPR_2019_PNI
Summary:
Inspired by the regularization of noise injection, this work designs the algorithm named Parametric Noise Injection to improve the robustness of the neural network. The proposed PNI technique is to inject layer-wise trainable Gaussian noise on various locations, including network input/activation/weights. For each inference, the injected noise is independently sampled from the corresponding Gaussian distribution, where its mean and variance of this distribution is trained by gradient descent method as other parameters of DNN.
Problem:

Many defense methods achieve robustness by using stochastic gradient, which can lead to a decrease of clean accuracy.
If the adopted method mainly performs the model regularization, it is expected to improve the perturbed-data accuracy without sacrificing the clean-data accuracy.
Key ideas:

By leveraging the regularization of noise injection to improve clean accuracy as well as robust accuracy.
Solutions:
Firstly, it defines the format of noise injection, which assigns a learnable parameter to the noise. Then it explores the back-propagation of this learnable parameter. And finally, it combines the PNI with adversarial training and minimizes the ensemble loss L′ which is the weighted sum of losses for clean- and perturbed-data.
Strengths & Weaknesses:
Strengths: Can improve the accuracy of AT.
Weaknesses: Must need the help of adversarial training to achieve robust accuracy improvement. It needs the ensemble loss to improve the clean accuracy.
Takeaways&How can I do better:

The theoretical analysis is valuable for our work.
