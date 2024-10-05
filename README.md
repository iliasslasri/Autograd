# Autograd

This is a simple non optimized implementation of auto diffrentiation with back-prop (reverse autodiff). It is not optimized for speed or memory usage. This is a simple implementation to understand the concept of autodiff and nn training.

Forwards and backwards pass are implemented for the following operations:
- Addition
- Subtraction
- Multiplication
- Division
- Power
- (more to come)

For the present time only scalar operations are supported.

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
[Value(data=0.9826529966007654, size=56Bytes),
 Value(data=0.000856126549434292, size=56Bytes),
 Value(data=0.9826529966007654, size=56Bytes)]
```

The only imports used in autodiff.ipynb are numpy, math and mathplotlib.