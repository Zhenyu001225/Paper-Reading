Title: [007][Robustness and Efficiency][Quantization and Robustness] Double-Win Quant: Aggressively Winning Robustness of Quantized Deep Neural Networks via Random Precision Training and Inference
Authors: Yonggan Fu, Qixuan Yu, Meng Li, Vikas Chandra, Yingyan Lin
Affiliations: Rice University
Publication Venue: ICML 2021
Link: http://proceedings.mlr.press/v139/fu21c.html
Code Link: https://github.com/RICE-EIC/Double-Win-Quant
Summary:
Problem:
The same idea as 2-in-1 work. From the experiments, it’s more difficult for adversarial attacks generated under one precision to fool the same adversarially trained model quantized to a different precision. How to leverage this phenomenon to boost DNN's robustness?
Key ideas:
Quantization noise can be leveraged to provide similar effects as permutations to the weights/activations and thus enhance DNNs’ robustness. Specifically, adversarial perturbations are shielded by the quantization noise between the two precisions, which can not be effectively learned by gradient-based attacks.
Solutions:
Random Precision Training(RPT) trains a model from scratch via randomly selecting a precision from a candidate set in each iteration for generating adversarial examples and updating the model with the selected precision while equipping the model with SBN to independently record the statistics of different precisions. Random Precision Inference(RPI) randomly selects one precision from an inference precision set to quantize the model’s weights and activations during inference.
Strengths & Weaknesses:
Strengths: Random brings noise.
Takeaways&How can I do better:
Like the random projection filters, the adversarial attack methods just adapt to the precision during training, not effective during inference with different precision.
