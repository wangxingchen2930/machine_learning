# Related Math

## Regularization

overall goal: to prevent overfitting

### L0, L1 & L2 regularization
- L0 and L1 can punish some 'useless' features to zero (**sparsity**) while L0 is more extreme than L1 which make it easier to push parameters to zero
- L1 example: LASSO (which solves the nondifferentiable of L1 norm)

## Entropy

- Entropy in information theory can be defined as the expected number of bits of information contained in an event.
- If the entropy is higher, that means we need more information to represent an event. 
- Entropy is considered as average bits of information required to represent an event drawn from the probability distribution.

### Cross-Entropy

- It is the average number of bits required to represent an event from one distribution, compared to another distribution.
- Cross-entropy is widely used in Deep Learning as a loss function to enable the learning. In that, the true probability distribution is the label and predicted distribution is the value from the current model.

### KL divergence

- We can define cross-entropy as the sum of entropy and KL divergence.
- KL divergence of zero indicates that two distribution are identica.

### Cross-Entropy vs KL divergence

- Cross-Entropy: Average number of total bits to represent an event from Q instead of P.
- Relative Entropy (KL Divergence): Average number of extra bits to represent an event from Q instead of P.