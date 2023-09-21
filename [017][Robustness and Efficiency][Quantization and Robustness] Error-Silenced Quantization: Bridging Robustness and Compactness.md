Title: [017][Robustness and Efficiency][Quantization and Robustness] Error-Silenced Quantization: Bridging Robustness and Compactness
Authors: Zhicong Tang , Yinpeng Dong and Hang Su
Affiliations: Tsinghua University
Venue: IJCAI 2020
Link: https://ceur-ws.org/Vol-2640/paper_8.pdf
Code Link: None
Summary:
Problem:
Quantization is found to weaken the robustness. But the adversarial training depends on the larger network capacity which contradicts with quantization. How to design an adversarial method for a quantization network to achieve both robustness and compactness?
Key ideas:
Silencing the Error Amplification Effect is the key to a robustness-aware quantization.
Solutions:
Combine the quantization loss and robustness loss, for the quantization, the method just apply a progressive quantization during the training, and for robustness, pairing activation is proposed.
Strengths & Weaknesses:
Strengths: It's another form of AT...
Weaknesses: A model that behaves closely on clean and adversarial inputs is supposed to gain close prediction accuracy on both. Is it correct???
Takeaways&How can I do better:
It's not reasonable.
