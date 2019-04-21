# apply


```python
DataFrame.apply(func, axis=0, broadcast=False, raw=False, reduce=None, args=(), **kwds)
```


```python
df = pd.DataFrame(np.arange(16).reshape((4,4)),index=['a','b','c','d'],columns=['one','two','three','four'])

def apply_func(arr):
	return arr['one'] + arr['two']

df['three'] =  df.apply(apply_func, axis = 1)

#讲第一列和第二列的数据相加，赋值到第3列
```

