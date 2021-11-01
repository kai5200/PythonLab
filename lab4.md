```python
import math
```


```python
math.floor(2.5)
```




    2




```python
math.ceil(2.5)
```




    3




```python
round(2.51)
```




    3




```python
round(2.5)
```




    2




```python
round(2.46)
```




    2




```python
pow(2,8)
```




    256




```python
math.pi
```




    3.141592653589793




```python
math.e
```




    2.718281828459045




```python
type(1+True)
```




    int




```python
type(1+True +2.0)
```




    float




```python
isinstance(6,str)
```




    False




```python
isinstance(6,(str,bool,int))
```




    True




```python
lst = list(range(5))
print(lst)
```

    [0, 1, 2, 3, 4]



```python
len(lst)
```




    5




```python
lst.count(2)
```




    1




```python
lst[4]
```




    4




```python
lst.append(10)
print(lst)
```

    [0, 1, 2, 3, 4, 10, 10, 10]



```python
lst.insert(-2,11)
print(lst)
```

    [0, 1, 2, 3, 4, 10, 11, 10, 10]



```python
print(lst)
lst1 = lst[0:3]
lst2 = lst[4:-1]
print(lst1)
print(lst2)
```

    [0, 1, 2, 3, 4, 10, 11, 10, 10]
    [0, 1, 2]
    [4, 10, 11, 10]



```python
lst1= lst1 *3
lst2 = lst2 + lst2
lst3 = lst1 + lst2 
print(lst1)
print(lst2)
print(lst3)
```

    [0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2]
    [4, 10, 11, 10, 4, 10, 11, 10, 4, 10, 11, 10, 4, 10, 11, 10, 4, 10, 11, 10, 4, 10, 11, 10, 4, 10, 11, 10, 4, 10, 11, 10]
    [0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 4, 10, 11, 10, 4, 10, 11, 10, 4, 10, 11, 10, 4, 10, 11, 10, 4, 10, 11, 10, 4, 10, 11, 10, 4, 10, 11, 10, 4, 10, 11, 10]



```python
lst3.clear()
print(lst3)
```

    []



```python
lst1.reverse()
print(lst1)
lst1.sort()
print(lst1)
```

    [0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2, 0, 1, 2]
    [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2, 2]



```python
lst0 = list(range(4))
lst2 = list(range(4))
print(lst0 == lst2)
print(id(lst0))
print(id(lst2))
```

    True
    140468309950080
    140468309947776



```python
triangle =[]
n = 6
for i in range(n):
    row=[1]
    triangle.append(row)
    if i == 0:
        continue
    for j in range(i-1):
        row.append(triangle[i-1][j]+triangle[i-1][j+1])
    row.append(1)
print(triangle)
```

    [[1], [1, 1], [1, 2, 1], [1, 3, 3, 1], [1, 4, 6, 4, 1], [1, 5, 10, 10, 5, 1]]



```python
triangle=[[1],[1,1]]
for i in range(2,6):
    cur = [1]
    pre = triangle[i-1]
    for j in range(len(pre)-1):
        cur.append(pre[j] + pre[j+1])
    cur.append(1)
    triangle.append(cur)
print(triangle)
```

    [[1], [1, 1], [1, 2, 1], [1, 3, 3, 1], [1, 4, 6, 4, 1], [1, 5, 10, 10, 5, 1]]



```python
n =6
oldline = []
newline = [1]
length = 0
print(newline)
for i in range(1,n):
    oldline = newline.copy()
    oldline.append(0)
    newline.clear()
    offset = 0
    while offset <= i:
        newline.append(oldline[offset-1] + oldline[offset])
        offset += 1
    print(newline)
```

    [1]
    [1, 1]
    [1, 2, 1]
    [1, 3, 3, 1]
    [1, 4, 6, 4, 1]
    [1, 5, 10, 10, 5, 1]



```python
n =6
oldline = []
newline = [1]
length = 0
print(newline)
for i in range(1,n):
    oldline = newline.copy()
    oldline.append(0)
    newline.clear()
    for j in range(i+1):
        newline.append(oldline[j-1] + oldline[j])
    print(newline)
```

    [1]
    [1, 1]
    [1, 2, 1]
    [1, 3, 3, 1]
    [1, 4, 6, 4, 1]
    [1, 5, 10, 10, 5, 1]



```python
import datetime

n = 1000000
pn = []
count = 0
start = datetime.datetime.now()
for x in range(2,n):
    for i in pn:
        count += 1
        if x % i ==0:
            break
    else:
        pn.append(x)
#print(pn)
print(len(pn))
print(count)
delta = (datetime.datetime.now() - start).total_seconds()
print (delta)

```

    78498
    3085786712
    277.983952



```python
import math
import datetime

n = 1000000
pn = []
count = 0
flag = False
start = datetime.datetime.now()
for x in range(2,n):
    for i in pn:
        count += 1
        if x % i ==0:  # no prime 
            flag = True
            break
        if i >= math.ceil(x ** 0.5): #prime
            flag = False 
            break
    if not flag:
        pn.append(x)
#print(pn)
print(len(pn))
print(count)
delta = (datetime.datetime.now() - start).total_seconds()
print (delta)

```

    78498
    14005898
    3.591468



```python
triangle = []
n=6
for i in range(n):
    row = [1]
    for k in range(i):
        row.append(1) if k == i-1 else row.append(0)
    triangle.append(row)
    if i == 0:
        continue
    for j in range(1, i//2 + 1):
        val = triangle[i-1][j-1] + triangle[i-1][j]
        row[j] = val
        if j != i - j:
            row[-j-1] = val
print(triangle)
```

    [[1], [1, 1], [1, 2, 1], [1, 3, 3, 1], [1, 4, 6, 4, 1], [1, 5, 10, 10, 5, 1]]



```python
triangle = []
n = 6

for i in range(n):
    row = [1]*(i+1)
    triangle.append(row)
    if i == 0:
        continue
    for j in range(1, i //2+1):
        val = triangle[i-1][j-1] + triangle[i-1][j]
        row[j] = val
        if j != i-j:
            row[-j-1]=val
print(triangle)
```

    [[1], [1, 1], [1, 2, 1], [1, 3, 3, 1], [1, 4, 6, 4, 1], [1, 5, 10, 10, 5, 1]]



```python
#tuple

t = tuple()
t = ()
print(t)
```

    ()



```python
t = tuple(range(1,10,2))
t
```




    (1, 3, 5, 7, 9)




```python
t=(2,3,5,6,3,4,2)
t
```




    (2, 3, 5, 6, 3, 4, 2)




```python
t=(1,)
t
```




    (1,)




```python
t=(1,)*5
t
```




    (1, 1, 1, 1, 1)




```python
t=(1,2,3)*6
t
```




    (1, 2, 3, 1, 2, 3, 1, 2, 3, 1, 2, 3, 1, 2, 3, 1, 2, 3)




```python

from collections import namedtuple
#Point = namedtuple('_Point',['x','y'])

Student = namedtuple('Student', 'name age')
tom = Student('tom', 20)
jerry = Student('jerry', 18)

print(tom.name)
print(tom.age)
print(jerry.name)
print(jerry.age)
```

    tom
    20
    jerry
    18



```python
# inoput 3 numbers, output sort 

nums = []
for i in range(3):
    nums.append(int (input('{}:'.format(i))))
    

```

    0:12
    1:15
    2:20



```python
#max min 

nums = []
out = None
for i in range(3):
    nums.append(int(input('{}:'.format(i))))
    
while True:
    cur = min(nums)
    print(cur)
    nums.remove(cur)
    if len(nums) == 1 :
        print(nums[0])
        break


```

    0:6
    1:99
    2:77
    6
    77
    99



```python
#sort 
nums=[]
out = None
for i in range(3):
    nums.append(int(input('{}:'.format(i))))
    
nums.sort()
print(nums)
```

    0:66
    1:88
    2:2100
    [66, 88, 2100]



```python
#bubble sort
num_list =[
    [1,23,55,66,11,3,4,990,5,21],
    [1, 3, 4, 5, 11, 21, 23, 55, 66, 990]
]
nums = num_list[0]
print(nums)
length = len(nums)
count_swap = 0
count = 0

for i in range(length):
    for j in range(length -i -1):
        count += 1
        if nums[j] > nums[j+1]:
            tmp = nums[j]
            nums[j] = nums[j+1]
            nums[j+1] = tmp
            count_swap += 1
print(nums,count_swap,count)

# for num_list[0] count_swap = 20 count =45
#for num_list[1] count_swap = 0 count = 45

```

    [1, 23, 55, 66, 11, 3, 4, 990, 5, 21]
    [1, 3, 4, 5, 11, 21, 23, 55, 66, 990] 20 45



```python
#bubble sort with flag
num_list =[
    [1,23,55,66,11,3,4,990,5,21],
    [1, 3, 4, 5, 11, 21, 23, 55, 66, 990,666,356,423]
]
nums = num_list[1]
print(nums)
length = len(nums)
flag = False 
count_swap = 0
count = 0

for i in range(length):
    flag = False
    for j in range(length -i -1):
        count += 1
        if nums[j] > nums[j+1]:
            tmp = nums[j]
            nums[j] = nums[j+1]
            nums[j+1] = tmp
            count_swap += 1
    if not flag:
        break
print(nums,count_swap,count)
```

    [1, 3, 4, 5, 11, 21, 23, 55, 66, 990, 666, 356, 423]
    [1, 3, 4, 5, 11, 21, 23, 55, 66, 666, 356, 423, 990] 3 12



```python
s1 = "I'm \ta super student"
print(s1)
```

    I'm 	a super student



```python
s1.split()
```




    ["I'm", 'a', 'super', 'student']




```python
s1.split('s')
```




    ["I'm \ta ", 'uper ', 'tudent']




```python
s1.split('super')
```




    ["I'm \ta ", ' student']




```python
s1.split('super ')
```




    ["I'm \ta ", 'student']




```python
s1.split(" ")
```




    ["I'm", '\ta', 'super', 'student']




```python
s1.split(' ', maxsplit=2)
```




    ["I'm", '\ta', 'super student']




```python
s1.split('\t', maxsplit=2)
```




    ["I'm ", 'a super student']




```python
s2 = """
this is an apple,
that is an orange.
i am xxx,
you are yyy.
"""
print(s2)
```

    
    this is an apple,
    that is an orange.
    i am xxx,
    you are yyy.
    



```python
print(s2.splitlines())
```

    ['', 'this is an apple,', 'that is an orange.', 'i am xxx,', 'you are yyy.']



```python
print(s2.splitlines(True))
```

    ['\n', 'this is an apple,\n', 'that is an orange.\n', 'i am xxx,\n', 'you are yyy.\n']



```python
s1.partition('s')
```




    ("I'm \ta ", 's', 'uper student')




```python
s1.partition('stu')
```




    ("I'm \ta super ", 'stu', 'dent')




```python
s1.partition(' ')
```




    ("I'm", ' ', '\ta super student')




```python
s1.title()
```




    "I'M \tA Super Student"




```python
s = "I am very very very sorry "
print(s)
```

    I am very very very sorry 



```python
s.strip()
```




    'I am very very very sorry'




```python
s.strip('Iy')
```




    ' am very very very sorry '




```python
s.strip('Iy ')
```




    'am very very very sorr'




```python
s.find('very')
```




    5




```python
s.find('very',-1)
#from right side , find nothing = -1
```




    -1




```python
s.index('very')
```




    5




```python
s.index('very',-1)
# value error 
```


    ---------------------------------------------------------------------------

    ValueError                                Traceback (most recent call last)

    <ipython-input-68-d494e791ef23> in <module>
    ----> 1 s.index('very',-1)
          2 # value error


    ValueError: substring not found



```python
len(s)
```




    26




```python
s.count('very')
```




    3




```python
s.startswith('very')
```




    False




```python
s.endswith('sorry')
```




    False




```python
s.startswith('very',5)
```




    True




```python
s.endswith('sorry',5,-1)
```




    True




```python

```
