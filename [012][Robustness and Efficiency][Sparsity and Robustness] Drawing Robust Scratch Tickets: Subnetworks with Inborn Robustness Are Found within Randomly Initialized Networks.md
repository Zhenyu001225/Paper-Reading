Title: [009][Robustness and Efficiency][Sparsity and Robustness] Drawing Robust Scratch Tickets: Subnetworks with Inborn Robustness Are Found within Randomly Initialized Networks
Authors: Yonggan Fu, Qixuan Yu, Yang Zhang, Shang Wu, Xu Ouyang, David Cox, Yingyan Lin
Affiliations: Rice University & MIT-IBM Watson AI Lab
Publication Venue: NeurIPS 2021
Link: https://proceedings.neurips.cc/paper/2021/file/6ce8d8f3b038f737cefcdafcf3752452-Paper.pdf
Code Link: https://github.com/RICE-EIC/Robust-Scratch-Ticket
Summary:
Problem:
Adversarial training might not be indispensable for adversarial robustness.
Key ideas:
Making the sparse network aware of robustness is the key idea of this paper, and it also uses the advantages of randomly weighted networks containing subnetworks. The location of weights holds most of the information encoded by the training, indicating that searching for the locations of a subset of weights within a randomly initialized network might be potentially as effective as adversarially training the weight values in generating a robust model.
Solutions:
Proposes a concept called RST, which is the subnetworks(sparse network) with robustness within any randomly initialized network without training for adversarial attack. In particular, in the min-max problem formulated in the paper, the parameters updated in the training process are not robust weights but sparse mask m. In addition, Random RST Switch is also put forward to ensure adversarial transferability between RSTs.
Strengths & Weaknesses:
Strengths: Let sparse parameter m obtain robust information, which achieves efficiency and robustness.
Weaknesses: Just considered the sparse weights. How about other parameters?
Takeaways&How can I do better:
This method is still essentially a form of adversarial training, except that it is a novel perspective of letting the sparse parameter m obtain robust information.
