- Perceptron implements the hyperplane
- Online (instances seen one by one) vs Batch (whole sample) learning:
- Stochastic Gradient Descent: Update weights after a single pattern such that the error is minimum for that specific pattern.
- Generic update rule (LMS Rule):
	- $$\nabla w_{ij}^{t}= \eta(r^{t}_{i}-y^{t}_{i})x^{t}_{j}$$
	- Update = Learning Factor ( Desired Output - Actual Output) input