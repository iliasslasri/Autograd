# Autograd

This is a simple non optimized implementation of auto diffrentiation with back-prop (reverse autodiff). It is not optimized for speed or memory usage. This is a simple implementation to understand the concept of autodiff and nn training.

In addittion to the autodiff, I implemented a simple neuron, layer and MLP with mse loss function. I used tanh as activation fct for all neurons.

This implemetation contains an example of training a simple neural net, with very simple training data.
```python
xs = [
    [2.0, 3.0, 1.0, 15.0],
    [1.0, 2.0, 3.0, 4.0],
    [3.0, 2.0, 1.0, 0.0]
]
target = [1.0, 0.0, 1.0]
```
Results of predictions after training are very good :
```python
[Value(data=0.9826529966007654),
 Value(data=0.000856126549434292),
 Value(data=0.9826529966007654)]
```

The only imports used in autodiff.ipynb are numpy, math and mathplotlib.
