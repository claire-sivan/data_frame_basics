```python
import pandas as pd 
df=pd.read_csv("C:\\Code\\pandas\\dataframe\\weather_data.csv")
```


```python
df
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
      <th>day</th>
      <th>temp</th>
      <th>windspeed</th>
      <th>event</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>01/01/2023</td>
      <td>32</td>
      <td>6</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>1</th>
      <td>01/02/2023</td>
      <td>35</td>
      <td>7</td>
      <td>Sunny</td>
    </tr>
    <tr>
      <th>2</th>
      <td>01/03/2023</td>
      <td>28</td>
      <td>2</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>3</th>
      <td>01/04/2023</td>
      <td>24</td>
      <td>7</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>4</th>
      <td>01/05/2023</td>
      <td>32</td>
      <td>4</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>5</th>
      <td>01/06/2023</td>
      <td>32</td>
      <td>2</td>
      <td>Sunny</td>
    </tr>
  </tbody>
</table>
</div>




```python
import pandas as pd 
df=pd.read_csv("weather_data.csv")
df
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
      <th>day</th>
      <th>temp</th>
      <th>windspeed</th>
      <th>event</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>01/01/2023</td>
      <td>32</td>
      <td>6</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>1</th>
      <td>01/02/2023</td>
      <td>35</td>
      <td>7</td>
      <td>Sunny</td>
    </tr>
    <tr>
      <th>2</th>
      <td>01/03/2023</td>
      <td>28</td>
      <td>2</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>3</th>
      <td>01/04/2023</td>
      <td>24</td>
      <td>7</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>4</th>
      <td>01/05/2023</td>
      <td>32</td>
      <td>4</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>5</th>
      <td>01/06/2023</td>
      <td>32</td>
      <td>2</td>
      <td>Sunny</td>
    </tr>
  </tbody>
</table>
</div>




```python
import pandas as pd
weather_data={ 
    'day':['01/01/2023','01/02/2023','01/03/2023','01/04/2023','01/05/2023','01/06/2023'],
    'temp':[32,35,28,24,32,32],
    'windspeed':[6,7,2,7,4,2],
    'event':['Rain','Sunny','Snow','Rain','Sunny']
}
df=pd.DataFrame()
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
      <th>day</th>
      <th>temp</th>
      <th>windspeed</th>
      <th>event</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>01/01/2023</td>
      <td>32</td>
      <td>6</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>1</th>
      <td>01/02/2023</td>
      <td>35</td>
      <td>7</td>
      <td>Sunny</td>
    </tr>
    <tr>
      <th>2</th>
      <td>01/03/2023</td>
      <td>28</td>
      <td>2</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>3</th>
      <td>01/04/2023</td>
      <td>24</td>
      <td>7</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>4</th>
      <td>01/05/2023</td>
      <td>32</td>
      <td>4</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>5</th>
      <td>01/06/2023</td>
      <td>32</td>
      <td>2</td>
      <td>Sunny</td>
    </tr>
  </tbody>
</table>
</div>




```python
# shape means the dimensions 
df. shape
```




    (6, 4)




```python
# tupple want to store the no of rows and columns 
rows,columns=df.shape 
```


```python
rows
```




    6




```python
columns
```




    4




```python
# this is how you print no of rows and columns
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
      <th>day</th>
      <th>temp</th>
      <th>windspeed</th>
      <th>event</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>01/01/2023</td>
      <td>32</td>
      <td>6</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>1</th>
      <td>01/02/2023</td>
      <td>35</td>
      <td>7</td>
      <td>Sunny</td>
    </tr>
    <tr>
      <th>2</th>
      <td>01/03/2023</td>
      <td>28</td>
      <td>2</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>3</th>
      <td>01/04/2023</td>
      <td>24</td>
      <td>7</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>4</th>
      <td>01/05/2023</td>
      <td>32</td>
      <td>4</td>
      <td>Rain</td>
    </tr>
  </tbody>
</table>
</div>




```python
# when you do not want to print the whole data frame 
df.head(2)

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
      <th>day</th>
      <th>temp</th>
      <th>windspeed</th>
      <th>event</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>01/01/2023</td>
      <td>32</td>
      <td>6</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>1</th>
      <td>01/02/2023</td>
      <td>35</td>
      <td>7</td>
      <td>Sunny</td>
    </tr>
  </tbody>
</table>
</div>




```python
# print the last 5 rows 
df.tail()
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
      <th>day</th>
      <th>temp</th>
      <th>windspeed</th>
      <th>event</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1</th>
      <td>01/02/2023</td>
      <td>35</td>
      <td>7</td>
      <td>Sunny</td>
    </tr>
    <tr>
      <th>2</th>
      <td>01/03/2023</td>
      <td>28</td>
      <td>2</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>3</th>
      <td>01/04/2023</td>
      <td>24</td>
      <td>7</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>4</th>
      <td>01/05/2023</td>
      <td>32</td>
      <td>4</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>5</th>
      <td>01/06/2023</td>
      <td>32</td>
      <td>2</td>
      <td>Sunny</td>
    </tr>
  </tbody>
</table>
</div>




```python
# last no in the tail
df.tail (2)
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
      <th>day</th>
      <th>temp</th>
      <th>windspeed</th>
      <th>event</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>4</th>
      <td>01/05/2023</td>
      <td>32</td>
      <td>4</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>5</th>
      <td>01/06/2023</td>
      <td>32</td>
      <td>2</td>
      <td>Sunny</td>
    </tr>
  </tbody>
</table>
</div>




```python
#print row no 2-5
df[2:5]
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
      <th>day</th>
      <th>temp</th>
      <th>windspeed</th>
      <th>event</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2</th>
      <td>01/03/2023</td>
      <td>28</td>
      <td>2</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>3</th>
      <td>01/04/2023</td>
      <td>24</td>
      <td>7</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>4</th>
      <td>01/05/2023</td>
      <td>32</td>
      <td>4</td>
      <td>Rain</td>
    </tr>
  </tbody>
</table>
</div>




```python
#print the columns 
df.columns

```




    Index(['day', 'temp', 'windspeed', 'event'], dtype='object')




```python
df.event

```




    0     Rain
    1    Sunny
    2     Snow
    3     Snow
    4     Rain
    5    Sunny
    Name: event, dtype: object




```python
df[['event','day','windspeed']]
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
      <th>event</th>
      <th>day</th>
      <th>windspeed</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Rain</td>
      <td>01/01/2023</td>
      <td>6</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Sunny</td>
      <td>01/02/2023</td>
      <td>7</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Snow</td>
      <td>01/03/2023</td>
      <td>2</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Snow</td>
      <td>01/04/2023</td>
      <td>7</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Rain</td>
      <td>01/05/2023</td>
      <td>4</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Sunny</td>
      <td>01/06/2023</td>
      <td>2</td>
    </tr>
  </tbody>
</table>
</div>




```python
df[['event','day','temp']]
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
      <th>event</th>
      <th>day</th>
      <th>temp</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Rain</td>
      <td>01/01/2023</td>
      <td>32</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Sunny</td>
      <td>01/02/2023</td>
      <td>35</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Snow</td>
      <td>01/03/2023</td>
      <td>28</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Snow</td>
      <td>01/04/2023</td>
      <td>24</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Rain</td>
      <td>01/05/2023</td>
      <td>32</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Sunny</td>
      <td>01/06/2023</td>
      <td>32</td>
    </tr>
  </tbody>
</table>
</div>




```python
df['temp']
```




    0    32
    1    35
    2    28
    3    24
    4    32
    5    32
    Name: temp, dtype: int64




```python
df['temp']
```




    <bound method Series.max of 0    32
    1    35
    2    28
    3    24
    4    32
    5    32
    Name: temp, dtype: int64>




```python
df['temp'].min
```




    <bound method Series.min of 0    32
    1    35
    2    28
    3    24
    4    32
    5    32
    Name: temp, dtype: int64>




```python
df['temp'].max()
```




    35




```python
df['temp'].mean()
```




    30.5




```python
df['temp'].min()
```




    24




```python
df['temp'].std()
```




    3.8858718455450894




```python
# print the statistics of those columns 
df.describe()

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
      <th>temp</th>
      <th>windspeed</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>6.000000</td>
      <td>6.000000</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>30.500000</td>
      <td>4.666667</td>
    </tr>
    <tr>
      <th>std</th>
      <td>3.885872</td>
      <td>2.338090</td>
    </tr>
    <tr>
      <th>min</th>
      <td>24.000000</td>
      <td>2.000000</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>29.000000</td>
      <td>2.500000</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>32.000000</td>
      <td>5.000000</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>32.000000</td>
      <td>6.750000</td>
    </tr>
    <tr>
      <th>max</th>
      <td>35.000000</td>
      <td>7.000000</td>
    </tr>
  </tbody>
</table>
</div>




```python
# conditionally select data
df[df.temp>=30]
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
      <th>day</th>
      <th>temp</th>
      <th>windspeed</th>
      <th>event</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>01/01/2023</td>
      <td>32</td>
      <td>6</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>1</th>
      <td>01/02/2023</td>
      <td>35</td>
      <td>7</td>
      <td>Sunny</td>
    </tr>
    <tr>
      <th>4</th>
      <td>01/05/2023</td>
      <td>32</td>
      <td>4</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>5</th>
      <td>01/06/2023</td>
      <td>32</td>
      <td>2</td>
      <td>Sunny</td>
    </tr>
  </tbody>
</table>
</div>




```python
df[df.'temp'=='temp'.max()]
```


      Cell In[42], line 1
        df[df.'temp'=='temp'.max()]
              ^
    SyntaxError: invalid syntax
    



```python
df.columns

```




    Index(['day', 'temp', 'windspeed', 'event'], dtype='object')




```python
df[df.temp==df.temp.max()]
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
      <th>day</th>
      <th>temp</th>
      <th>windspeed</th>
      <th>event</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1</th>
      <td>01/02/2023</td>
      <td>35</td>
      <td>7</td>
      <td>Sunny</td>
    </tr>
  </tbody>
</table>
</div>




```python
df[df.temp==temp.max()]
```


```python
df.columns

```




    Index(['day', 'temp', 'windspeed', 'event'], dtype='object')




```python
df[df.temp==df['temp'].max()]
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
      <th>day</th>
      <th>temp</th>
      <th>windspeed</th>
      <th>event</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1</th>
      <td>01/02/2023</td>
      <td>35</td>
      <td>7</td>
      <td>Sunny</td>
    </tr>
  </tbody>
</table>
</div>




```python
# print the day when temp was maximum 
df[['day']df.temp==df['temp'].max()]
```


      Cell In[51], line 2
        df[['day']df.temp==df['temp'].max()]
           ^
    SyntaxError: invalid syntax. Perhaps you forgot a comma?
    



```python
df['day'][df.temp==df['temp'].max()]
```




    1    01/02/2023
    Name: day, dtype: object




```python
df.columns

```




    Index(['day', 'temp', 'windspeed', 'event'], dtype='object')




```python
df[['day','temp']][df.temp==df['temp'].max()]
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
      <th>day</th>
      <th>temp</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1</th>
      <td>01/02/2023</td>
      <td>35</td>
    </tr>
  </tbody>
</table>
</div>




```python
#index
df
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
      <th>day</th>
      <th>temp</th>
      <th>windspeed</th>
      <th>event</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>01/01/2023</td>
      <td>32</td>
      <td>6</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>1</th>
      <td>01/02/2023</td>
      <td>35</td>
      <td>7</td>
      <td>Sunny</td>
    </tr>
    <tr>
      <th>2</th>
      <td>01/03/2023</td>
      <td>28</td>
      <td>2</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>3</th>
      <td>01/04/2023</td>
      <td>24</td>
      <td>7</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>4</th>
      <td>01/05/2023</td>
      <td>32</td>
      <td>4</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>5</th>
      <td>01/06/2023</td>
      <td>32</td>
      <td>2</td>
      <td>Sunny</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.index
```




    RangeIndex(start=0, stop=6, step=1)




```python
df.columns
```




    Index(['day', 'temp', 'windspeed', 'event'], dtype='object')




```python
df.set_index('day')
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
      <th>temp</th>
      <th>windspeed</th>
      <th>event</th>
    </tr>
    <tr>
      <th>day</th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>01/01/2023</th>
      <td>32</td>
      <td>6</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>01/02/2023</th>
      <td>35</td>
      <td>7</td>
      <td>Sunny</td>
    </tr>
    <tr>
      <th>01/03/2023</th>
      <td>28</td>
      <td>2</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>01/04/2023</th>
      <td>24</td>
      <td>7</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>01/05/2023</th>
      <td>32</td>
      <td>4</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>01/06/2023</th>
      <td>32</td>
      <td>2</td>
      <td>Sunny</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.set_index('event')
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
      <th>day</th>
      <th>temp</th>
      <th>windspeed</th>
    </tr>
    <tr>
      <th>event</th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Rain</th>
      <td>01/01/2023</td>
      <td>32</td>
      <td>6</td>
    </tr>
    <tr>
      <th>Sunny</th>
      <td>01/02/2023</td>
      <td>35</td>
      <td>7</td>
    </tr>
    <tr>
      <th>Snow</th>
      <td>01/03/2023</td>
      <td>28</td>
      <td>2</td>
    </tr>
    <tr>
      <th>Snow</th>
      <td>01/04/2023</td>
      <td>24</td>
      <td>7</td>
    </tr>
    <tr>
      <th>Rain</th>
      <td>01/05/2023</td>
      <td>32</td>
      <td>4</td>
    </tr>
    <tr>
      <th>Sunny</th>
      <td>01/06/2023</td>
      <td>32</td>
      <td>2</td>
    </tr>
  </tbody>
</table>
</div>




```python
df
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
      <th>day</th>
      <th>temp</th>
      <th>windspeed</th>
      <th>event</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>01/01/2023</td>
      <td>32</td>
      <td>6</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>1</th>
      <td>01/02/2023</td>
      <td>35</td>
      <td>7</td>
      <td>Sunny</td>
    </tr>
    <tr>
      <th>2</th>
      <td>01/03/2023</td>
      <td>28</td>
      <td>2</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>3</th>
      <td>01/04/2023</td>
      <td>24</td>
      <td>7</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>4</th>
      <td>01/05/2023</td>
      <td>32</td>
      <td>4</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>5</th>
      <td>01/06/2023</td>
      <td>32</td>
      <td>2</td>
      <td>Sunny</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.set_index('day',inplace=True)
```


```python
df

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
      <th>temp</th>
      <th>windspeed</th>
      <th>event</th>
    </tr>
    <tr>
      <th>day</th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>01/01/2023</th>
      <td>32</td>
      <td>6</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>01/02/2023</th>
      <td>35</td>
      <td>7</td>
      <td>Sunny</td>
    </tr>
    <tr>
      <th>01/03/2023</th>
      <td>28</td>
      <td>2</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>01/04/2023</th>
      <td>24</td>
      <td>7</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>01/05/2023</th>
      <td>32</td>
      <td>4</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>01/06/2023</th>
      <td>32</td>
      <td>2</td>
      <td>Sunny</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.loc['01/04/2023']
```




    temp           24
    windspeed       7
    event        Snow
    Name: 01/04/2023, dtype: object




```python
df.reset_index(inplace=True)
```


```python
df.reset_index(inplace=True)
df
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
      <th>index</th>
      <th>day</th>
      <th>temp</th>
      <th>windspeed</th>
      <th>event</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>01/01/2023</td>
      <td>32</td>
      <td>6</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>01/02/2023</td>
      <td>35</td>
      <td>7</td>
      <td>Sunny</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>01/03/2023</td>
      <td>28</td>
      <td>2</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3</td>
      <td>01/04/2023</td>
      <td>24</td>
      <td>7</td>
      <td>Snow</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4</td>
      <td>01/05/2023</td>
      <td>32</td>
      <td>4</td>
      <td>Rain</td>
    </tr>
    <tr>
      <th>5</th>
      <td>5</td>
      <td>01/06/2023</td>
      <td>32</td>
      <td>2</td>
      <td>Sunny</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.set_index('event',inplace=True)
```


```python
df
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
      <th>index</th>
      <th>day</th>
      <th>temp</th>
      <th>windspeed</th>
    </tr>
    <tr>
      <th>event</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Rain</th>
      <td>0</td>
      <td>01/01/2023</td>
      <td>32</td>
      <td>6</td>
    </tr>
    <tr>
      <th>Sunny</th>
      <td>1</td>
      <td>01/02/2023</td>
      <td>35</td>
      <td>7</td>
    </tr>
    <tr>
      <th>Snow</th>
      <td>2</td>
      <td>01/03/2023</td>
      <td>28</td>
      <td>2</td>
    </tr>
    <tr>
      <th>Snow</th>
      <td>3</td>
      <td>01/04/2023</td>
      <td>24</td>
      <td>7</td>
    </tr>
    <tr>
      <th>Rain</th>
      <td>4</td>
      <td>01/05/2023</td>
      <td>32</td>
      <td>4</td>
    </tr>
    <tr>
      <th>Sunny</th>
      <td>5</td>
      <td>01/06/2023</td>
      <td>32</td>
      <td>2</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.loc['Snow']
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
      <th>index</th>
      <th>day</th>
      <th>temp</th>
      <th>windspeed</th>
    </tr>
    <tr>
      <th>event</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Snow</th>
      <td>2</td>
      <td>01/03/2023</td>
      <td>28</td>
      <td>2</td>
    </tr>
    <tr>
      <th>Snow</th>
      <td>3</td>
      <td>01/04/2023</td>
      <td>24</td>
      <td>7</td>
    </tr>
  </tbody>
</table>
</div>




```python
df
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
      <th>index</th>
      <th>day</th>
      <th>temp</th>
      <th>windspeed</th>
    </tr>
    <tr>
      <th>event</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Rain</th>
      <td>0</td>
      <td>01/01/2023</td>
      <td>32</td>
      <td>6</td>
    </tr>
    <tr>
      <th>Sunny</th>
      <td>1</td>
      <td>01/02/2023</td>
      <td>35</td>
      <td>7</td>
    </tr>
    <tr>
      <th>Snow</th>
      <td>2</td>
      <td>01/03/2023</td>
      <td>28</td>
      <td>2</td>
    </tr>
    <tr>
      <th>Snow</th>
      <td>3</td>
      <td>01/04/2023</td>
      <td>24</td>
      <td>7</td>
    </tr>
    <tr>
      <th>Rain</th>
      <td>4</td>
      <td>01/05/2023</td>
      <td>32</td>
      <td>4</td>
    </tr>
    <tr>
      <th>Sunny</th>
      <td>5</td>
      <td>01/06/2023</td>
      <td>32</td>
      <td>2</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.reset_index(inplace=True)
df
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
      <th>event</th>
      <th>index</th>
      <th>day</th>
      <th>temp</th>
      <th>windspeed</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Rain</td>
      <td>0</td>
      <td>01/01/2023</td>
      <td>32</td>
      <td>6</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Sunny</td>
      <td>1</td>
      <td>01/02/2023</td>
      <td>35</td>
      <td>7</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Snow</td>
      <td>2</td>
      <td>01/03/2023</td>
      <td>28</td>
      <td>2</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Snow</td>
      <td>3</td>
      <td>01/04/2023</td>
      <td>24</td>
      <td>7</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Rain</td>
      <td>4</td>
      <td>01/05/2023</td>
      <td>32</td>
      <td>4</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Sunny</td>
      <td>5</td>
      <td>01/06/2023</td>
      <td>32</td>
      <td>2</td>
    </tr>
  </tbody>
</table>
</div>




```python

```
