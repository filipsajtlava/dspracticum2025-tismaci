# Trying out various combinations of parameters

- started with CNN that looked like this (convolution part):
```bash
3 -> 16 (kernel 3x3 with padding) -> 16 (kernel 3x3 no padding)
```
- neural net part with (image went from 28*28 to 26\*26 because of the convolution with no padding):
```bash
26x26x16 -> 128 -> 6
```

|learning rate $\gamma$ | act. $f$ type | # of epochs | test accuracy (approx.)| 
|----|----|---|--:|
|0.02| ReLU| 5 | 25% | 
|0.10| ReLU| 5 | $\gamma$ too high
|0.06| ReLU | 5| 43% |
|0.06| ReLU | 5 + dropout| 25% (not enough data to need dropout probably)|
|0.06| ReLU | 10 | 48%|

### Adding another layer of neurons:
```bash
26x26x26 -> 128 -> 64 -> 6
```
|learning rate $\gamma$ | act. $f$ type | # of epochs | test accuracy (approx.)| 
|----|----|---|--:|
|0.06| ReLU| 5 | 32% |
|0.02| ReLU| 5 | 38% | 
|0.01 | ReLU | 10 | 47%|
|0.01 |ReLU | 20 | 48% |


In this casethe learning rate was better off being smaller.

### Simplifying the model
```bash
26x26x26 -> 64 -> 6
```
