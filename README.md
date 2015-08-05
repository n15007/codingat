# Codingat
## Warmup-1
### sleep_in
> "weekday""vacation"というパラメータがあります。祝日か休日ならTrueを返す。
```
def sleep_in(weekday, vacation):
  return (not weekday or vacation)
```


### monkey_trouble
> a と bと言う猿が2匹います。一匹がsmileでもう一匹がnot smileならトラブルになる。
```
def monkey_trouble(a_smile, b_smile):
  return (a_smile == b_smile)
```

### sum_double
> 2つの値があり、異なった値なら合計、同じ値なら合計の2倍の値を返す。
```
def sum_double(a, b):
  sum = a + b
  if a == b:
   sum = sum * 2
  return sum
```
  

