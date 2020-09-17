# PROG-7
```python
def integrate(f: Callable[[float], float],
              a: float, b: float, n_iter: int = 1000,
              accuracy: int = 8) -> float:
    return round(sum(tuple(map(f, tuple(a + float((b - a) / n_iter) * n for n in range(n_iter))))) *
                 float((b - a) / n_iter), accuracy)
```
