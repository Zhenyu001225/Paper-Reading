Title: [004][Robustness and Efficiency][Quantization and Robustness] Defensive Quantization: When Efficiency Meets Robustness
Authors: Ji Lin, Chuang Gan, Song Han
Affiliations: MIT
Publication Venue: ICLR 2019
Link: https://arxiv.org/abs/1904.08444
Code Link: None
Summary:
Problem:
The conventional quantization approaches are vulnerable to adversarial attacks because of the error amplification effect. How to address this problem and jointly optimize the efficiency and robustness of deep learning models by using quantization?
Key ideas:
Control the Lipschitz constant of the network during quantization by adding a Lipschitz Regularization to the loss function, such that the magnitude of the adversarial noise remains non-expansive during inference.
Solutions:
Firstly, this paper defined how Lipschitz constant works in keeping the network a non-expansive network. Then, from the perspective of math, this problem is transformed into a spectral norm, which is the maximum singular value of weight. But computing the singular values of each weight matrix is not computationally feasible during training, so this problem is further transformed into matrix form and added to the loss function as ||W^T* W - I||^2.
Strengths & Weaknesses:
Strengths:  Easy to operate and understand; When in a low-bit situation, DQ can improve the robustness by about 40%.
Takeaways&How can I do better:
Quantization helps robustness in the low perturbation strength. This phenomenon is worth doing research.
