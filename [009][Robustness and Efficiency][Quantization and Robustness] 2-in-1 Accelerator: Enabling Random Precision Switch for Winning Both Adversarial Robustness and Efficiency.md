Title: [006][Robustness and Efficiency][Quantization and Robustness] 2-in-1 Accelerator: Enabling Random Precision Switch for Winning Both Adversarial Robustness and Efficiency
Authors: Yonggan Fu, Yang Zhao, Qixuan Yu, Chaojian Li, Yingyan Lin
Affiliations: Rice University
Publication Venue: MICRO 2021
Link: https://dl.acm.org/doi/abs/10.1145/3466752.3480082
Code Link: None
Summary:
Problem:
From the experiments, it’s more difficult for adversarial attacks generated under one precision to fool the same adversarially trained model quantized to a different precision. How to leverage this phenomenon to boost DNN's robustness?
Key ideas:
Quantization noise can be leveraged to provide similar effects as permutations to the weights/activations and thus enhance DNNs’ robustness.
Solutions:
An algorithm called Random Precision Switch (RPS) and the corresponding accelerator are invented to win robustness as well as efficiency. In particular, RPS can effectively defend DNNs against adversarial attacks by enabling random DNN quantization as an in-situ model switch during training and inference. According to the algorithm's features, this paper also designs a precision-scalable accelerator, which addresses the dilemma between flexibility and performance by combining the temporal and spatial designs, reduces the area of shift-add logic, and comes out with a more comprehensive optimizer for dataflow.
Strengths & Weaknesses:
Strengths: Random brings noise.
Takeaways&How can I do better:
Like the random projection filters, the adversarial attack methods just adapt to the precision during training, not effective during inference with different precision. 
