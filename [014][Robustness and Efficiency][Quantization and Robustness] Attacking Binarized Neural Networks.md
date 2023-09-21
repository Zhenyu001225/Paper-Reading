Title: [002][Robustness and Efficiency][Quantization and Robustness] Attacking Binarized Neural Networks
Authors: Angus Galloway, Graham W. Taylor, Medhat Moussa
Affiliations: University of Guelph, Canada 
Venue: ICLR 2018
Link:https://arxiv.org/abs/1711.00449
Code Link: https://github.com/AngusG/cleverhans-attacking-bnns
Summary:
Problem:
Why does very low quantization have robustness outperforming the original model? 
Key ideas:
From the experiments, this paper proposed one possible explanation for this property is that higher quantization introduces higher amounts of non-linearity, which prevents small changes in the input from drastically altering the output and forcing a misclassification.
Takeaways&How can I do better:
Think about how Dmi bring noise and non-linearity?
