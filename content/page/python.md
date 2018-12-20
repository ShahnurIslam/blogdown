---
title: "Python"
date: 2018-12-18T15:36:35Z
subtitle: ""
tags: [python]
---

# Table of Contents
* [Pandas](##Pandas)
  * [Pandas Conditonal Column](#Pandas Conditonal Column)
[//]: <> (2. [SQL Windows Function](#SQL Windows Function))

## Pandas
### Pandas Conditonal Column

A conditional column is a column in a dataframe that is generated based on other column/s. There are multiple way of doing this in Python but one of the quickest ways is to use the `np.where()` function. This function is basically the equivalent of an if statement in Excel.

`np.where(condition,True action, False action)`

``` {python}
#import the two libraries
import numpy as np
import pandas as pd

#generate a pandas dataframe of one column with a 100 random integers
df = pd.DataFrame(np.random.randint(low=0,high = 100,size = (100,1)),columns = ['col1'])

#Generate a conditional column that checks if the number is even or odd
df['odd/even'] = np.where(df['col1'] % 2 == 1, 'odd', 'even')
```
If we print the first 5 rows of our data frame we get :

       col1 odd/even
    0    87      odd
    1    85      odd
    2    22     even
    3    80     even
    4     0     even

    
    

[//]: <> (## SQL Windows Function)

