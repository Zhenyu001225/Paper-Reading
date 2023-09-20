Title: [006][Robustness and Efficiency][Approximation and Robustness] Adversarial Robustness via Random Projection Filters
Authors: Minjing Dong, Chang Xu
Affiliations: University of Sydney
Publication Venue: CVPR 2023
Link: https://openaccess.thecvf.com/content/CVPR2023/html/Dong_Adversarial_Robustness_via_Random_Projection_Filters_CVPR_2023_paper.html
Code Link: https://github.com/UniSerj/Random-Projection-Filters
Summary:
Problem:
Defending white-box attacks needs to involve some noise during the network inference, which can significantly influence the optimization. How to achieve a trade-off between robustness and optimization?
Key ideas:
A bunch of filters are selected as the Random Projection Filters, and the rest still remain traditional filters. In this way, the former is responsible for defense, and the latter tries to keep the accuracy. RPF's parameters are randomly sampled during adversarial training and inference, which means that parameters in RPF can't be approximated by the attack methods. 
Solutions:
Replace a bunch of the convolutional filters in CNN layers with random projection because intuitively, a higher ratio of random projection in CNNs could make it difficult for white-box attackers to obtain adversarial perturbations while also bringing huge noise to network optimization. In particular, this work divides the filter in CNN into two parts, the first Nr filters are the random projection filters with parameters randomly sampled from a Gaussian distribution, and the rest is the traditional convolutional operation.
Adversarial examples are produced from a network with random projection filters F1:Nr [A] and then the adversarial examples are used to train a network with random projection filters F1:Nr [I]. F1:Nr [A] is re-sampled and becomes F1:Nr [I] during evaluation so that X_adv can hardly be generalized to fθ[I].
Strengths & Weaknesses:
Strengths: CNNs can perform a strong defense during the inference phase.
Takeaways&How can I do better:
The attack methods in the experiments; The defense methods in the experiments.
