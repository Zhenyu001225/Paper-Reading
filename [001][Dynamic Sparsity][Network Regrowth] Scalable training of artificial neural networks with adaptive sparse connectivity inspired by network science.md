Title: [001][Dynamic Sparsity][Network Regrowth] Scalable training of artificial neural networks with adaptive sparse connectivity inspired by network science//
Authors: Decebal Constantin Mocanu, Elena Mocanu, Peter Stone, Phuong H. Nguyen, Madeleine Gibescu, Antonio Liotta
Affiliations: Eindhoven University of Technology
Publication Venue: Nature Communication 2018
Link: https://www.nature.com/articles/s41467-018-04316-3
Code Link: https://github.com/dcmocanu/sparse-evolutionary-artificial-neural-networks
Summary:
Problem:
How can artificial neural networks mimic biological neural networks' sparse topological features? Two main challenges: how to prune and re-add the weights properly without decreasing the accuracy.
Key ideas:
Motivated by the network properties of biological neural networks, Sparse Evolutionary Training (SET) proposes a simple scheme where weights are pruned according to the standard magnitude criterion used in pruning and are added back at random.
Solutions:
Specifically, SET replaces the fully-connected layer(FC) with the sparse-connected layer(SC) at first. In each training epoch, when performing weights update, it removes a fraction of the smallest positive and largest negative weights. If the epoch is not the last one, weights are added randomly in the same amount as the ones previously removed.
Strengths:
Experiments on RBMs, MLPs, and CNN prove that SET reduces quadratically the number of parameters, with no decrease in accuracy, and even outperforms.
Takeaways&Weaknesses&How can I do better:
Is it too coarse-grained to add weights randomly, with each weight having a different level of importance or even a different level of significance per layer? This is similar to doing a Random Walk in a search space.
