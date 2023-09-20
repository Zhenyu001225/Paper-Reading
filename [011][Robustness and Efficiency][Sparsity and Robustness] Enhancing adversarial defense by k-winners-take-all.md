Title: [011][Robustness and Efficiency][Sparsity and Robustness] Enhancing adversarial defense by k-winners-take-all
Authors: Chang Xiao, Peilin Zhong, Changxi Zheng
Affiliations: Columbia University
Publication Venue: ICLR 2020
Link: https://arxiv.org/abs/1905.10510
Code Link: https://github.com/a554b554/kWTA-Activation
Summary:
Problem:
The most effective way of finding such a perturbation (or adversarial example) is by exploiting the gradient information of the network with respect to its input. Most of the existing robust methods prefer to hide the gradients, which can be always approximated by the attack methods. How to defend the gradient-based attack more effectively without hiding the gradient?
Key ideas:
k-WTA advocates the use of k-Winners-Take-All (k-WTA) activation to produce sparse activation. From the perspective of mathematics, sparse activations mainly make the gradient undefined, through which the gradient-based attack method can't approximate or reproduce the model's gradient.
Solutions:
k-WTA achieves the defense of the gradient-based attack methods by using a sparse activation function called k-WTA function, which just keeps the k-th largest activation value while other values are set to zero.
Strengths & Weaknesses:
Strengths: Can adapt to universal network arch and training methods; Without any retraining; Outperformed the ReLU on white-box attack.
Weaknesses: Performed not so well in Black-Box attack situation; Defend only gradient-based attack methods.
Takeaways&How can I do better:
Experiments Settings.
