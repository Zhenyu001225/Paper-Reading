Title: [003][Robustness and Efficiency][Sparsity and Robustness] Robust Binary Models by Pruning Randomly-initialized Networks
Authors: Chen Liu, Ziqi Zhao, Sabine Süsstrunk Mathieu Salzmann
Affiliations: EPFL
Venue: NeurIPS 2022
Link: https://proceedings.neurips.cc/paper_files/paper/2022/file/035f23c0ac4cf2b73b9365ba5a98ad56-Paper-Conference.pdf
Code Link: https://github.com/IVRL/RobustBinarySubNet
Summary:
Problem:
Robustness to adversarial attacks needs a large memory footprint. This paper aims to achieve robust yet compact models.
Key ideas:
Like the Robust Scratch Ticket, this method injects robust information into the neural network sparsity. But this method obtains better performance and a more stable training behavior than RST by adding two components.
Solutions:
Firstly, it initializes the model parameters as either +1 or 1, keeps them fixed, and finds a subnetwork structure that is robust to attacks. Specifically, the binary mask code is found by the adversarial training with the updating of binary mask m. And develops an adaptive pruning strategy to adaptively use different pruning rates for different layers. Furthermore, introduces a normalization-based technique to increase the algorithm’s stability for binary networks.
Strengths & Weaknesses:
Strengths: Binary neural network brings more compression;  Adaptive pruning.
Weaknesses: Its results are similar with the results from AT.
Takeaways&How can I do better:
The comparison with other methods in this paper can be referred to. 
