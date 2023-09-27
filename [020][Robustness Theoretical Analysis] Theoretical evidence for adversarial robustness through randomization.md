Title: [020][Robustness Theoretical Analysis] Theoretical evidence for adversarial robustness through randomization
Authors: Rafael Pinot, Laurent Meunier, Alexandre Araujo, Hisashi Kashima, Florian Yger1 Cédric Gouy-Pailler, Jamal Atif 
Affiliations: Université Paris-Dauphine, PSL Research University, CNRS, LAMSADE, Paris, France
Publication Venue: NeurIPS 2019
Link:https://proceedings.neurips.cc/paper_files/paper/2019/hash/36ab62655fa81ce8735ce7cfdaf7c9e8-Abstract.html
Summary:
Problem:
Provide the theoretical proof for the noise injection robustness improvement.
Key ideas:
Limiting the gap between risk under standard inference and the risk under adversarial attack. In this way, in the neuron network's training process, it naturally has robustness.
Solutions:
Mainly focus on the proof of the theorem 2. Firstly, it defines the risk in the standard training process, as well as the risk under adversarial scenarios. Then this paper gives a detailed definition of adversarial robustness, which needs the metrics/divergence on the probabilistic mapping. Finally, it proves that if the noise injected into the network is sampled from the exponential family, it has a trade-off between clean accuracy and robustness.
Takeaways&How can I do better:
DMI is a kind of noise injection, which this theoretical analysis can support.
We can refer to this as our algorithm's theoretical analysis.
