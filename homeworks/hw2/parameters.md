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
|0.06| ReLU | 15| 37% |

### Adding another layer of neurons:
```bash
26x26x16 -> 128 -> 128 -> 6
```
|learning rate $\gamma$ | act. $f$ type | # of epochs | test accuracy (approx.)| 
|----|----|---|--:|
|0.01| ReLU| 15 | 38% |
|0.01| ReLU| 30 | 39% |
|0.01| ReLU| 45 | 42% |
|0.03| ReLU | 15| 38% |

### Simplifying the model
```bash
26x26x16 -> 64 -> 6
```

|learning rate $\gamma$ | act. $f$ type | # of epochs | test accuracy (approx.)| 
|----|----|---|--:|
|0.02| ReLU| 5 | 18% |
|0.06| ReLU| 5 | 28% | 

```bash
26x26x26 -> 256 -> 6
```

|learning rate $\gamma$ | act. $f$ type | # of epochs | test accuracy (approx.)| 
|----|----|---|--:|
|0.06| ReLU| 5 | 28% | 
|0.01| ReLU| 15 | 36% |
|0.01| ReLU| 30 | 45% |

```bash
26x26x26 -> 512 -> 6
```

|learning rate $\gamma$ | act. $f$ type | # of epochs | test accuracy (approx.)| 
|----|----|---|--:|
|0.01| ReLU| 15 | 34% |
|0.01| ReLU| 30 | 42%|
|0.01| ReLU | 45 | 49%|
|0.01| ReLU | 60 | 54%|

### Created a new dataset
Containing only 5 different classes (as opposed to the original 6) with more training images (around 300 * 0.75 per class)
```bash
3 -> 16 (kernel 3x3 with padding) -> 16 (kernel 3x3 no padding) -> 26x26x16 -> 128 -> 5
```

|learning rate $\gamma$ | act. $f$ type | # of epochs | test accuracy (approx.)| 
|----|----|---|--:|
|0.02| ReLU| 5 | 43% | 
|0.02| ReLU| 10 | 52% | 
|0.02| ReLU| 15 | 48% |

-> started overfitting at 15 epochs, going to try drop-out with 15% chance
|learning rate $\gamma$ | act. $f$ type | # of epochs | test accuracy (approx.)| 
|----|----|---|--:|
|0.02| ReLU| 5 | 48% | 
|0.02| ReLU| 10 | 49% | 
|0.02| ReLU| 15 | 53% | 
|0.02| ReLU| 20 | 52% | 

-> started overfitting a bit later, set drop-out to 25%
|learning rate $\gamma$ | act. $f$ type | # of epochs | test accuracy (approx.)| 
|----|----|---|--:|
|0.02| ReLU| 5 | 43% | 
|0.02| ReLU| 15 | 54% | 
|0.02| ReLU| 20 | 37% | 

-> still very mediocre
```bash
3 -> ... -> 512 -> 5 (no drop-out)
```
|learning rate $\gamma$ | act. $f$ type | # of epochs | test accuracy (approx.)| 
|----|----|---|--:|
|0.02| ReLU| 5 | 43% |
|0.02| ReLU| 10 | 56% |  
|0.02| ReLU| 15 | 51% | 

-> guessing that in case of 4x as many neurons some drop-out might help with the overfitting (setting it to 15% again)

|learning rate $\gamma$ | act. $f$ type | # of epochs | test accuracy (approx.)| 
|----|----|---|--:|
|0.02| ReLU| 15 | 52% |
|0.04| ReLU| 15 | 57% |
|0.04| ReLU| 20 | 52% |
|0.06| ReLU| 15 | 22% |

```bash
3 -> 32 (kernel 3x3 with padding) -> 32 (kernel 3x3 no padding) -> 26x26x32 -> 512 -> 5
```

|learning rate $\gamma$ | act. $f$ type | # of epochs | test accuracy (approx.)| 
|----|----|---|--:|
|0.02| ReLU| 5 |46% |
|0.02| ReLU| 10 |49% |
|0.02| ReLU| 15 |57% |
|0.02| ReLU | 30 | 61%|