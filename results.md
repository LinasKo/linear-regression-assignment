# Results
All results used 50 epochs.

### Fixed bias; No regularisation
The gradient descent makes increasingly long jumps if learning rate > e-7.
Setting it to e-7 allowed it to converge successfully, with test accuracy of **0.744**.
Setting learning rate to e-9 or below makes the algorithm not reach the optimal state.

### Learned bias; Regularisation
Strangely enough, the learned **b** parameter remained close to 0. The accuracy barely improved to **0.747**

### Regularisation
Regularisation does not seem to affect the problem here, except on extreme values of 1e6, when it makes the model not converge again.

### Final Remarks
I think I see why data normalisation is so important. I feel like if I had done that, playing around with both regularisation and learning rate would have been easier.
