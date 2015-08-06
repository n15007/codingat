# Codingat
## Warmup-1
### sleep_in
> "weekday""vacation"というパラメータがあります。祝日か休日ならTrueを出力する。
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
> 2つの値があり、異なった値なら合計、同じ値なら合計の2倍の値を出力する。
```
def sum_double(a, b):
  sum = a + b
  if a == b:
   sum = sum * 2
  return sum
```

### diff21
> 21 と n の絶対値を求める。n が 21 を越したら絶対値の2倍を出力する。
```
def diff21(n):
  a = 21 - n
  if n > 21:
   a = (n - 21) * 2
  return a
  ```
  
### parrot_trouble
> おしゃべりオウムがいます。7時~20時の間にオウムが喋るとトラブルになる。
```
def parrot_trouble(talking, hour):
  return(talking and not(hour >= 7 and hour <= 20))
```

### makes10
> a と b の2つの整数のどちらかが 10 または2つを足して 10 なら True を出力する。
```
def makes10(a, b):
  return((a == 10 or b == 10) or (a + b == 10))
```

### near_hundred
> 整数 n があります。100 または 200 と n の絶対値が10以内なら True を出力する。
```
def near_hundred(n):
  return(abs(100 -n) <= 10 or abs(200 - n) <= 10)
```

### pos_neg
> 両方が negative または not negative なら True を出力する。
```
def pos_neg(a, b, negative):
    if negative:
     return(a < 0 and b < 0)
    else:
     return((a < 0 and b > 0) or (a > 0 and b < 0))
```

### not_string
> 文字列の最初に not があったらそのまま出力、なかったら not を前に追加して出力する。
```
def not_string(str):
  if len(str) >= 3 and str[:3] == 'not':
   return str
  return 'not ' + str
```

### missing_char
> 文字が入ってる文字列と整数 n があります。 n 番目の文字を消して新しく文字を出力する。
```
def missing_char(str, n):
  front = str[:n]
  back = str[n+1:]
  return front + back
```

### front_back
> 文字列があります。最初と最後の1文字を入れ替えて出力する。
```
def front_back(str):
    if len(str) <= 1:
     return str
     mid = str[1:-1]
    return str[len(str)-1] + mid + str[0]
```

### front3
> 文字列があります。文字列に入ってる最初の3文字を3回繰り替えして出力する。
```
def front3(str):
  front = str[:3]
  return front + front + front
```

### string_times
> nの数だけ文字列を続け表示する。
```
def string_times(str, n):
  moji = ''
  for x in range(n):
    moji = moji + str
  return moji
```

### front_times
> 文字列の最所の3文字をn回繰り替えして表示する。
```
def string_times(str, n):
  moji = ''
  for x in range(n):
    moji = moji + str
  return moji
```

### string_bits
> 文字列の最所の文字の次の文字から1つずつ飛ばして表示する。
```
def string_bits(str):
  moji = ''
  for x in range(len(str)):
   if x % 2 == 0:
    moji = moji + str[x]
  return moji
```

### string_splosion
> 文字列の 'Code' 'CCoCodCode' と表示する。
```
def string_splosion(str):
  moji = ''
  for i in range(len(str)):
   moji = moji + str[:i+1]
  return moji
```

### last2
> 文字列の最後の2文字より前の文字が最後の2文字と同じ文字をカウントする。
```
def last2(str):
  if len(str) < 2:
   return 0
  last = str[-2:]
  count = 0
  for i in range(len(str)-2):
   sub = str[i:i+2]
   if sub == last:
    count += 1
  return count
```

### array_count9
> ある整数の配置の中に数字の９が何個あるかカウントする。
```
def array_fount9(nums):
  count = 0
  for i in nums:
   if i == 9:
    count += 1
  return count
```

### array123
> ある整数の配置に"1, 2, 3"と続いていたらTrueを出力する。。
```
def array123(nums):
  for i in range(len(nums)-2):
   if nums[i] == 1 and nums[i+1] == 2 and nums[i+2] == 3:
    return True
  return False
```

### string_match
> a b の2つの文字列があり、同じ位置に同じ2文字があればカウントする。
```
def string_match(a, b):
  str = min(len(a), len(b))
  count = 0
  for i in range(str - 1):
   a2 = a[i:i+2]
   b2 = b[i:i+2]
   if a2 == b2:
    count += 1
  return count
```
