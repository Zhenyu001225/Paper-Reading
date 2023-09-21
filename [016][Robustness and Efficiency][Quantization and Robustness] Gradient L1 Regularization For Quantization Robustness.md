Title: [016][Robustness and Efficiency][Quantization and Robustness] Gradient L1 Regularization For Quantization Robustness
Authors: Milad Alizadeh, Arash Behboodi, Mart van Baalen, Christos Louizos, Tijmen Blankevoort, and Max Welling
Affiliations: Qualcomm AI Research
Venue: ICLR 2020
Link: https://arxiv.org/abs/2002.07520
Code Link: None
Summary:
Problem:
How to solve the quantization amplified error of the adversarial perturbation to bring more robustness and accuracy?
Key ideas:
Model the quantization noise as a perturbation bounded in the `L∞-norm.
Solutions:
Firstly, this method models the quantization noise( brought by quantization and adversarial perturbation) into a kind of L-1 norm regularization. Specifically, it defined the output perturbation as the multiplication of quantization bit-width and the gradient of weights as well as the activation respectively. In this way, L-1 norm regularization can be added to the final loss function.
Strengths & Weaknesses:
Strengths: Provide a new perspective of the output perturbation. In the very low-bit quantization situation, this method outperforms DQ.
Takeaways&How can I do better:
Think of the DMI's optimization idea.
