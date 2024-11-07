## `round()`

> **摘自官方文档**：For the built-in types supporting [`round()`](https://docs.python.org/3/library/functions.html#round "round"), values are rounded to the closest multiple of 10 to the power minus _ndigits_; if two multiples are equally close, rounding is done toward the even choice (so, for example, both `round(0.5)` and `round(-0.5)` are `0`, and `round(1.5)` is `2`). Any integer value is valid for _ndigits_ (positive, zero, or negative). The return value is an integer if _ndigits_ is omitted or `None`. Otherwise, the return value has the same type as _number_.


> 也称银行家舍入  
### examples：
```python
# round(number, ndigits);round half to even
print(round(6.5))  # 输出: 6
print(round(7.5))  # 输出: 8
```
---


