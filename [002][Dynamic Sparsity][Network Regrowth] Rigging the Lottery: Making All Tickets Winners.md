Title: [002][Dynamic Sparsity][Network Regrowth] Rigging the Lottery: Making All Tickets Winners
Authors: Utku Evci, Trevor Gale, Jacob Menick, Pablo Samuel Castro, Erich Elsen
Affiliations: Google Brain & DeepMind
Publication Venue: ICLR 2020
Link: http://proceedings.mlr.press/v119/evci20a/evci20a.pdf
Code Link: https://github.com/google-research/rigl
Summary:
Problem:
How to quantify the importance of weights in an appropriate way to make space search more directional?
Key ideas:
RigL improves the optimization of sparse neural networks by leveraging weight magnitude and gradient information to jointly optimize model parameters and connectivity.
Solutions:
Similar to SET, RigL still removes weights close to 0 when sparsifying. But when doing regrowth, RigL performs top-k sorting on the saved gradients and only takes the top-k connections with larger gradients for regrowth.
Takeaways&Weaknesses&How can I do better:
Sparsity initialization method like ERK has some impact on the result, which means that considering the importance layer also works.
