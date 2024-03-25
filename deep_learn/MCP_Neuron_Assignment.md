```python
## mcp neuron(McCulloch and Walter Pitts)
```


```python
def mcp_neuron(inputs, weights, threshold, operation):
    if operation == 'and':
        result = all(x >= w for x, w in zip(inputs, weights))
    elif operation == 'or':
        result = any(x >= w for x, w in zip(inputs, weights))
    else:
        raise ValueError("Invalid operation. Please choose 'and' or 'or'.")


    return 1 if result >= threshold else 0
```


```python
mcp_neuron([0,1],[1,1],1,"or")
```




    1




```python

```
