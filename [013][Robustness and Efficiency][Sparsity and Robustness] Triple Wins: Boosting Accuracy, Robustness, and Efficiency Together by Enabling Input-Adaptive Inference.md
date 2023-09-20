Title: [001][Robustness and Efficiency][Sparsity and Robustness] Triple Wins: Boosting Accuracy, Robustness, and Efficiency Together by Enabling Input-Adaptive Inference Authors: Ting-Kuei Hu,Tianlong Chen, Haotao Wang, Zhangyang Wang 
Affiliations: Texas A&M University Publication 
Venue: ICLR 2020
Link: https://arxiv.org/abs/2002.10025
Code Link: https://github.com/TAMU-VITA/triple-wins
Summary:
Problem:
Key ideas:
Like the ensemble, it allows for each input (either clean or adversarial) to adaptively choose one of the multiple output layers (early branches or the final one) to output its prediction. Early exit ensures efficiency, multiple branches keep the accuracy, and robustness is achieved by three forms of adversarial attacks and their corresponding defense methods.
Solutions:
First augment the network with multiple early-branch output layers in addition to the original final output. Each input, regardless of clean or adversarial samples, adaptively chooses which output layer to take for its own prediction. Therefore, a large portion of input inferences can be terminated early when the samples can already be inferred with high confidence.RDI set an early threshold to achieve efficiency. And this method adds adversarial training in the loss function. The final optimal objective is the fusion of these two functions.
Strengths & Weaknesses:
Strengths: Early exit saves much resources.
Weaknesses: Need adversarial training; loss function is complicated.
Takeaways&How can I do better:
It's just the combination of early exit and adversarial training.
