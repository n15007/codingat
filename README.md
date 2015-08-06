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

### diff21
> 21 から　n　を
```
def diff21(n):
  a = 21 - n
  if n > 21:
   a = (n - 21) * 2
  return a
  ```
  
### parrot_trouble
> おしゃべりオウムがいます。
```
def parrot_trouble(talking, hour):
  return(talking and not(hour >= 7 and hour <= 20))
```

### makes10
> a と b の2つの整数が
```
def makes10(a, b):
  return((a == 10 or b == 10) or (a + b == 10))
```

### near_hundred
> 整数 n 
```
def near_hundred(n):
  return(abs(100 -n) <= 10 or abs(200 - n) <= 10)
```

### pos_neg
> 2つの値がありま。
```
def pos_neg(a, b, negative):
    if negative:
     return(a < 0 and b < 0)
    else:
     return((a < 0 and b > 0) or (a > 0 and b < 0))
```

### not_string
> 文字列があります
```
def not_string(str):
  if len(str) >= 3 and str[:3] == 'not':
   return str
  return 'not ' + str
```

### missing_char
> ほにゃららら
```
def missing_char(str, n):
  front = str[:n]
  back = str[n+1:]
  return front + back
```

### front_back
> 文字列があります。
```
def front_back(str):
    if len(str) <= 1:
     return str
     mid = str[1:-1]
    return str[len(str)-1] + mid + str[0]
```

### front3
> aaaaaa
```
def front3(str):
  front = str[:3]
  return front + front + front
```



  

