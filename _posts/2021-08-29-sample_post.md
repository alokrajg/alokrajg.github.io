---
published: true
categories: [data_science]
tags:
  - data_science
title: Jupyter notebook post
---

```python
import numpy as np
import pandas as pd
```

## create numpy array
```python
a = np.arange(1,200,4)
```


```python
df = pd.DataFrame(a)
df.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>0</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
    </tr>
    <tr>
      <th>1</th>
      <td>5</td>
    </tr>
    <tr>
      <th>2</th>
      <td>9</td>
    </tr>
    <tr>
      <th>3</th>
      <td>13</td>
    </tr>
    <tr>
      <th>4</th>
      <td>17</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.plot()
```




    <AxesSubplot:>




    
![png](\assets\images\sample_post\o.png)
    



```python

```
