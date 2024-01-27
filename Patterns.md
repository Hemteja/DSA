# 1


```python
n = 5
for i in range(n):
    print('*' * n)
```

    *****
    *****
    *****
    *****
    *****
    

# 2


```python
n = 5

count = 1
for i in range(n):
    print('*' * count)
    count += 1
```

    *
    **
    ***
    ****
    *****
    

# 3


```python
n = 6

num = 1
for i in range(n):
    for j in range(1,num):
        print(j , end = "")
    num += 1
    print()
```

    
    1
    12
    123
    1234
    12345
    

# 4


```python
n = 5

num = 1
for i in range(n):
    print(str(num) * (i + 1), end = "")
    print()
    num += 1
```

    1
    22
    333
    4444
    55555
    

# 5


```python
n = 5

for i in range(n):
    print('*' * n)
    n -= 1
```

    *****
    ****
    ***
    **
    *
    

# 6


```python
n = 5

num = 6
for i in range(n):
    for j in range(1,num):
        print(j, end = "")
    num -= 1
    print()
```

    12345
    1234
    123
    12
    1
    

# 7


```python
n = 5

count = 1
for i in range(1,n+1):
    print(" " * (n - i) + '*' * count)
    count += 2
```

        *
       ***
      *****
     *******
    *********
    

# 8


```python
n = 5

count = (n * 2) - 1
for i in range(1,n+1):
    print(" " * (i - 1) + "*" * count)
    count -= 2
```

    *********
     *******
      *****
       ***
        *
    

# 9


```python
n = 5

count = -1
for i in range(1,n+1):
    count += 2
    print(" " * (n - i) + "*" * count)
    
for i in range(1,n+1):
    print(" " * (i-1) + "*" * count)
    count -= 2
```

        *
       ***
      *****
     *******
    *********
    *********
     *******
      *****
       ***
        *
    

# 10


```python
n = 5

for i in range(1,n+1):
    print("*" * i)

for i in range(1,n):
    print("*" * (n-i))
```

    *
    **
    ***
    ****
    *****
    ****
    ***
    **
    *
    

# 11


```python
n = 5

for i in range(1,n+1):
    if i % 2 == 0:
        init = 0
    else:
        init = 1
    
    for j in range(i):
        print(init , end = " ")
        if init == 0:
            init = 1
        else:
            init = 0
    print()
```

    1 
    0 1 
    1 0 1 
    0 1 0 1 
    1 0 1 0 1 
    

# 12


```python
n = 4

num = 1
string = "1"
for i in range(1,n+1):
    print(string + " " * ((n - i) * 2) + string[::-1])
    num += 1
    string += str(num)
```

    1      1
    12    21
    123  321
    12344321
    

# 13


```python
n = 6

num = 1
for i in range(1,n):
    for j in range(i):
        print(num , end = " ")
        num += 1
    print()
```

    1 
    2 3 
    4 5 6 
    7 8 9 10 
    11 12 13 14 15 
    

# 14


```python
n = 5

for i in range(1,n+1):
    num = 65
    for j in range(i):
        print(chr(num) , end = "")
        num += 1
    print()
```

    A
    AB
    ABC
    ABCD
    ABCDE
    

# 15


```python
n = 5

for i in range(n):
    num = 65
    for j in range(n-i):
        print(chr(num) , end = "")
        num += 1
    print()
```

    ABCDE
    ABCD
    ABC
    AB
    A
    

# 16


```python
n = 5

num = 65
for i in range(1,n+1):
    for j in range(i):
        print(chr(num), end = "")
    print()
    num += 1
```

    A
    BB
    CCC
    DDDD
    EEEEE
    

# 17


```python
n = 5

for i in range(1,n+1):
    num = 65
    string = ''
    for j in range(i):
        string += chr(num)
        num += 1
    print(" " * (n-i) + string + string[:-1][::-1])
```

        A
       ABA
      ABCBA
     ABCDCBA
    ABCDEDCBA
    

# 18


```python
n = 5

for i in range(1,n+1):
    string = ''
    num = 65
    for j in range(i):
        string += chr(num + (n - i))
        num += 1
    print(string)    
```

    E
    DE
    CDE
    BCDE
    ABCDE
    

# 19


```python
n = 5

count = 5
space = 0
for i in range(n):
    print("*" * count + " " * space + "*" * count)
    count -= 1
    space += 2
    
for i in range(n):
    count += 1
    space -= 2
    print("*" * count + " " * space + "*" * count)
```

    **********
    ****  ****
    ***    ***
    **      **
    *        *
    *        *
    **      **
    ***    ***
    ****  ****
    **********
    

# 20


```python
n = 5

for i in range(1,n+1):
    print("*" * i + " " * ((n - i) * 2) + "*" * i)

for i in range(1,n):
    print("*" * (n-i) + " " * (2 * i) + "*" * (n-i))
```

    *        *
    **      **
    ***    ***
    ****  ****
    **********
    ****  ****
    ***    ***
    **      **
    *        *
    

# 21


```python
n = 6

for i in range(1,n+1):
    if i == 1 or i == n:
        print("*" * n)
        print()
    else:
        print("*" + " " * (n-2) + "*")
        print()
```

    ******
    
    *    *
    
    *    *
    
    *    *
    
    *    *
    
    ******
    
    

# 22


```python
n = 5

total = int((n * 2) / 2)
lst = []

for row in range(total):
    string = ''
    for col in range(total):
        string += str(n - min(row,col))
    lst.append(string)
    
for i in range(len(lst)):
    print(*(lst[i] + lst[i][:-1][::-1]))
for i in range(2,len(lst)+1):
    print(*(lst[-i] + lst[-i][:-1][::-1]))
```

    5 5 5 5 5 5 5 5 5
    5 4 4 4 4 4 4 4 5
    5 4 3 3 3 3 3 4 5
    5 4 3 2 2 2 3 4 5
    5 4 3 2 1 2 3 4 5
    5 4 3 2 2 2 3 4 5
    5 4 3 3 3 3 3 4 5
    5 4 4 4 4 4 4 4 5
    5 5 5 5 5 5 5 5 5
    


```python

```
