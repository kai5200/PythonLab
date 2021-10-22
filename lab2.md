```python
flag = 10
while flag:  # 0 false then while stop
    print("Flag = "+str(flag))
    flag -= 1
```

    Flag = 10
    Flag = 9
    Flag = 8
    Flag = 7
    Flag = 6
    Flag = 5
    Flag = 4
    Flag = 3
    Flag = 2
    Flag = 1



```python
for i in range(10):
    print(i+1)
```

    1
    2
    3
    4
    5
    6
    7
    8
    9
    10



```python
a = range(0,10,3)
list(a)
```




    [0, 3, 6, 9]




```python
for i in range(10):
    print(10-i)
```

    10
    9
    8
    7
    6
    5
    4
    3
    2
    1



```python
for i in range(10):
    if i%2:
        #continue
        print (i)
```

    1
    3
    5
    7
    9
    11
    13
    15
    17
    19



```python
for i in range(10):
    if not i%2:
        print (i)
```

    0
    2
    4
    6
    8



```python
count = 0  #reset count 
for i in range(0,1000,7):
    print (i)
    count += 1
    if count == 10:
        break
```

    0
    7
    14
    21
    28
    35
    42
    49
    56
    63



```python
count = 0
i = 0
while True:
    print (i)
    i += 7 
    count += 1
    if count == 10: #9th 7 step
        break
```

    0
    7
    14
    21
    28
    35
    42
    49
    56
    63



```python
val = int(input (">>>Give me a number: "))
print (val)
count = 0
while True:
    print(val%10)
    val = val // 10
    count += 1
    if val == 0:
        break
print("there are {} numbers ".format(count))
```

    >>>Give me a number: 4039920889
    4039920889
    9
    8
    8
    0
    2
    9
    9
    3
    0
    4
    there are 10 numbers 



```python
val = input("Give me a nuber ")
print ("your number is",val)
val1 = len(val)
#print (val1)
val2 = list(val)
#print (val2)
print ("this is {} number".format(val1))
for i in range(0,val1):
    print(val2[i])
```

    Give me a nuber 677
    your number is 677
    this is 3 number
    6
    7
    7



```python

```
