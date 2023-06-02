```python
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns; sns.set()
```


```python
def relu(arr):
    return ( (arr > 0) * arr)
```


```python
xs = np.linspace(-10, 10, 10_000)
plt.plot(xs, relu(xs))
```




    [<matplotlib.lines.Line2D at 0x7fc49bb4d4f0>]




    
![png](output_2_1.png)
    



```python
def dev_relu(arr):
    return (arr > 0) * np.ones(arr.shape)
```


```python
plt.plot(xs, dev_relu(xs))
```




    [<matplotlib.lines.Line2D at 0x7fc458142400>]




    
![png](output_4_1.png)
    


### One Layer


```python
def func(x, y):
    x_noise = x + np.random.normal(loc=0, scale=1)
    y_noise = y + np.random.normal(loc=0, scale=1)
    return x_noise**2 + y_noise
```


```python
np.meshgrid(np.linspace(-10, 10, 10_000), np.linspace(-10, 10, 10_000))
```




    [array([[-10.       ,  -9.9979998,  -9.9959996, ...,   9.9959996,
               9.9979998,  10.       ],
            [-10.       ,  -9.9979998,  -9.9959996, ...,   9.9959996,
               9.9979998,  10.       ],
            [-10.       ,  -9.9979998,  -9.9959996, ...,   9.9959996,
               9.9979998,  10.       ],
            ...,
            [-10.       ,  -9.9979998,  -9.9959996, ...,   9.9959996,
               9.9979998,  10.       ],
            [-10.       ,  -9.9979998,  -9.9959996, ...,   9.9959996,
               9.9979998,  10.       ],
            [-10.       ,  -9.9979998,  -9.9959996, ...,   9.9959996,
               9.9979998,  10.       ]]),
     array([[-10.       , -10.       , -10.       , ..., -10.       ,
             -10.       , -10.       ],
            [ -9.9979998,  -9.9979998,  -9.9979998, ...,  -9.9979998,
              -9.9979998,  -9.9979998],
            [ -9.9959996,  -9.9959996,  -9.9959996, ...,  -9.9959996,
              -9.9959996,  -9.9959996],
            ...,
            [  9.9959996,   9.9959996,   9.9959996, ...,   9.9959996,
               9.9959996,   9.9959996],
            [  9.9979998,   9.9979998,   9.9979998, ...,   9.9979998,
               9.9979998,   9.9979998],
            [ 10.       ,  10.       ,  10.       , ...,  10.       ,
              10.       ,  10.       ]])]




```python

```
