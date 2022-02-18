# 18.02.2022

###Задача 1###

    s = input().split()
    for i in range(0, len(s), 2):
    print(s[i])

###Задача 2###

    a = input().split()
    for i in range(0, len(a)):
    if int(a[i]) % 2 == 0:
    print(a[i], end=' ')

Задача 3

    a = map(int, input().split())
    n = 0
    for i in a:
    if i > 0:
    n += 1
    print(n)

Задача 4

     s = [int(i) for i in input().split()]
     for i in range(1, len(s)):
     if s[i] > s[i - 1]:
     print(s[i])

Задача 5

    s = [int(i) for i in input().split()]
    for i in range(1, len(s)):
   if s[i - 1] * s[i] > 0:
   print(s[i - 1], s[i])
  break

Задача 6

    s = [int(i) for i in input().split()]
    counter = 0
    for i in range(1, len(s) - 1):
    if s[i - 1] < s[i] > s[i + 1]:
    counter += 1
    print(counter)

Задача 7

    index_of_max = 0
    s = [int(i) for i in input().split()]
    for i in range(1, len(s)):
    if s[i] > s[index_of_max]:
    index_of_max = i
    print(s[index_of_max], index_of_max)

Задача 8

    i=list(input().split())
    min=1000
    for k in range(len(i)):
    s=int(i[k])
    if (s<min)and(s>0):
    min=s
    print(min)

Задача 9

    num = list(map(int, input().split()))
   min= 0
   for i in range(len(num)):
   if num[i] % 2 == 1:
   min= num[i]
    break
    for i in range(len(num)):
    if num[i] % 2 == 1:
    if num[i] < min:
    min = num[i]
    if min != 0:
     print(min)
    else:
    print(0)

Задача 10

     a = [int(s) for s in input().split()]
     n = int(input())
    for i in range(len(a)):
     if n > a[i]:
     print(i+1)
     break
     elif i == len(a)-1:
     print(len(a)+1)
