---
title: "Hello canals in Southeast Asian peatlands increase carbon emissions"
collection: publications
permalink: /publication/canals
excerpt: 'This paper presents a novel convolutional neural network to detect canals and study the effect of canals on land subsidence.'
date: 2021-03-23
venue: 'AGU Advances'
paperurl: 'https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2020AV000321'
citation: 'Dadap, N. C., Hoyt, A. M., Cobb, A. R., Oner, D., Kozinski, M., Fua, P. V., <b>Rao, K.</b>, Harvey, C. F., & Konings, A. G. (2021). Drainage Canals in Southeast Asian Peatlands Increase Carbon Emissions. AGU Advances, 2(1), e2020AV000321. https://doi.org/10.1029/2020AV000321'
---

Tropical peatlands are swamp‐like environments in which naturally wet conditions slow the decomposition of plant carbon that would otherwise be released to the atmosphere. However, over the past few decades, humans have built drainage canals in Southeast Asian peatlands, due to economic pressure for logging and agriculture. These canals are a major threat to peatlands because they dry out peat soils, in turn speeding up decomposition and making soils susceptible to wildfire. Both of these mechanisms release massive amounts of carbon dioxide to the atmosphere, thereby accelerating climate change. Despite these risks, until now the extent of drainage in peatlands was unknown due to a lack of drainage canal maps. Here, we create the first regional map of drainage canals by training a computer algorithm to identify canals within high‐resolution satellite images. We find that drainage is widespread—occurring in at least 65% of Southeast Asian peatlands. Furthermore, we find that more drainage canals are related to progressively larger subsidence rates—deformations in the ground surface partly caused by carbon dioxide emissions to the atmosphere. These findings suggest that it is important to know where and how much drainage is occurring to accurately predict subsidence and target areas for restoration.

q


_Canal segmentation results_


```python
pip install numpy
```

    Collecting numpy
      Downloading numpy-1.21.2-cp39-cp39-macosx_10_9_x86_64.whl (17.0 MB)
    [K     |████████████████████████████████| 17.0 MB 4.8 MB/s eta 0:00:01
    [?25hInstalling collected packages: numpy
    Successfully installed numpy-1.21.2
    Note: you may need to restart the kernel to use updated packages.



```python
import numpy as np
x = np.array([[100],
              [100]])
A = np.array([[1.05, 0],
              [0,    1.03]])
A.dot(x)
```




    array([[105.],
           [103.]])




```python
A.dot(A.dot(x))
```




    array([[110.25],
           [106.09]])




```python
from numpy import linalg as lg
l = lg.eigvals(A)
print(l)
```

    [1.05 1.03]



```python
print("Hello World")
```

    Hello World



```python

```

```

<style>
table, tr, td ,th{
   border: none!important;
}
</style>

<hr>
<body class="sponsored">

<h2 class="centered"> Research graciously funded by</h2>

<table >
  <tr >
    <td ><a class="greyed" href="https://www.eng.ed.ac.uk/" target="_blank"> <img src="https://ahmadbelb.github.io/Blog/images/ed.png"  alt="1" width = 500px ></a></td>

    <td><a class="greyed" href="https://www.Arup.com/" target="_blank"><img src="https://ahmadbelb.github.io/Blog/images/Arup.png" alt="2" width = 360px ></a></td>
 <td><a class="greyed" href="https://www.transport.gov.scot/" target="_blank"><img src="https://ahmadbelb.github.io/Blog/images/scot.png" alt="2" width = 400px ></a></td>
   </tr> 
   <tr>
    

     
  </tr>
</table>
</body>

