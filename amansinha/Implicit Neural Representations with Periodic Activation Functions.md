# Implicit Neural Representations with Periodic Activation Functions

Paper Link: (https://arxiv.org/pdf/2006.09661.pdf)

The paper talks about conventional practise of generalization in neural networks and  its incapability of distinguishing between different arcitechtures based on the generalization performance. 

The work presents collections of investigations about the idea of neural nets to fit on datasets in a generalized fashion. These includes various randomization tests such replacing true labels with random labels in complete and partial manner; putting noise into the inputs from zero to completely replacing inputs from Gaussian distribution.

Replacing true labels with randomized labels was based on the intuition that model may not be able to converge or slowly converge. But, experiments showeed that models were unaffected with this change.
Similar case happened in the case of put noise into inputs.  

The main findings are:

* While regularization is important, bigger gains can be achieved by simply changing the model architecture. It is difficult to say that the regularizers count as a fundamental phase change in the generalization capability of deep nets.

* Explicit and implicit regularizers are consistently suggesting that regularizers, when properly tuned, could help to improve the generalization performance. However, it is unlikely that the regularizers are the fundamental reason for generalization, as the networks continue to perform well after all the regularizers removed.

* As soon as the number of parameters p of a networks is greater than n, even simple two-layer neural networks can represent any function of the input sample.

* Preprocessing like applying Gaussian Kernel is order to minimise the norm also is not a predictive of model performance, as in irrespective of the l_2 norm, generization may still vary.


The randomization experiments showed that the effective capacity of several successful neural network architectures is large enough to shatter the training data. This situation poses a conceptual challenge to statistical learning theory as traditional measures of model complexity struggle to explain the generalization ability of large artificial neural networks. 

This poses question that why optimization continues to be empirically easy even if the resulting model does not generalize, which can be extended to the hypothesis that cause of generalization must be different from cause of optimization.
