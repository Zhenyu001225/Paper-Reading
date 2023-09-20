Title: [005][Robustness and Efficiency][Quantization and Robustness] Empir: Ensembles of mixed precision deep networks for increased robustness against adversarial attacks
Authors: Sanchari Sen, Balaraman Ravindran, Anand Raghunathan
Affiliations: Purdue University
Publication Venue: ICLR 2020
Link: https://arxiv.org/pdf/2004.10162.pdf
Code Link: https://github.com/sancharisen/EMPIR
Summary:
Problem:
Quantized neural networks often demonstrate much higher robustness to adversarial attacks than full precision networks, but at the cost of a substantial loss in accuracy on the original (unperturbed) inputs. How to address this problem to achieve efficiency and robustness simultaneously? 
Key ideas:
The higher unperturbed accuracies of the full precision models combined with the higher robustness of the low precision models, by composing them in an ensemble.
Solutions:
An EMPIR model comprises M full-precision (FP) models which help in boosting the unperturbed accuracy of the overall model and N low-precision (LP) models which contribute towards higher robustness. All the individual models are fed the same input and their predicted classes or probabilities are combined with the help of an ensembling technique at the end to determine the final prediction of the EMPIR model.
Strengths & Weaknesses:
Strengths: Easy to deploy
Weaknesses: Averaging and max voting ensemble tech just considers the final output; Too many models to do the EMPIR, and each model's acc is still not good.
Takeaways&How can I do better:
Ensemble technique.
How about other ensemble functions?
