### Role of Cost Functions in NRL NTWRKS

- Is a metric for evaluating how effective the network is and for informing us what we need to tweak within the model so that it performs better within the context of our data

### MAE

- This is also known as L1 norm

### MSE

- Also known as L2 norm
- More sensitive to outliers
- Should be used for regression since it derives from an idea of a normal distribution 

### MAE vs MSE

One way to think about MAE is that all errors are weighted equally. 

MSE weights outliers more strongly. The larger the discrepancy, the more the model is penalised. 
- In situations where outliers are potentially fatal (like driving) a cost function that is "hard" on outliers so to speak can be more rewarding

MSE is continuously differentiable, whereas MAE is not differentiable when our input is equal to our output

### Why not Lin Reg for Classification?

When we use linear regression for more than 2 classes, we tell the model that some class has a higher value than another class. We implicitly create this "ordering" as tibshrani put it, and we can't reasonably conclude this without a good reason. 
- Lin reg could be used in binary classification cases, but it's good to consider this and think about it

Questions:
- MSE vs MAE for neural networks
- Is MSE and MAE ok to use for neural networks when we are attemping to do classification?

### Common issues with MAE
- MAE, while continuous is not continuously differentiable due to its absolute value properties
	- Recall that the limit of the absolute value function doesn't exist at 0
- This causes issues when we try to calculate the derivative during backpropogation
- MSE can be more helpful
	- Or if we're not that concerned about the edge case, we can just code in the hard case for MAE
