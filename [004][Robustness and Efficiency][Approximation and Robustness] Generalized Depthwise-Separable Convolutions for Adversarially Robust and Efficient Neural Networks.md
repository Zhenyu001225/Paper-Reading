Title: [004][Robustness and Efficiency][Approximation and Robustness] Generalized Depthwise-Separable Convolutions for Adversarially Robust and Efficient Neural Networks
Authors: Hassan Dbouk & Naresh R. Shanbhag
Affiliations: University of Illinois at Urbana-Champaign
Publication Venue: NeurIPS 2021
Link: https://proceedings.neurips.cc/paper_files/paper/2021/file/649adc59afdef2a8b9e943f94a04b02f-Paper.pdf
Code Link: https://github.com/hsndbk4/GDWS
Summary:
Problem:
Many works have explored the model compression of CNN but neglect the throughput and robustness of it. How to achieve the efficiency and robustness of CNN simultaneously? 
Key ideas:
Conventional depth-separable convolution assigns only one kernel on each channel, which greatly reduces the accuracy of the approximation for 2D convolution. The method proposed in this paper increases the number of kernels on each channel, improving the accuracy of the approximation.
Solutions:
After defining the GDWS method, this paper proposed the optimal GDWS Approximation method, which aims to lower the error between 2D convolution and GDWS. Specifically, it uses the Frobenius norm of a matrix to minimize the weighted approximation error. In addition, the complexity error is introduced to be controlled.
Strengths & Weaknesses:
Strengths: Improves the throughput; doesn't require any additional training.
Weaknesses: mainly focus on throughput improvement, while robustness improvement is too limited.
Takeaways&How can I do better:
Can't improve robustness, just focus on the throughput improvement without influencing the robustness.
