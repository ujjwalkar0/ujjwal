---
title: "Algorithm :  Thousand Separator"
subtitle: Source :-
  https://leetcode.com/contest/biweekly-contest-33/problems/thousand-separator/
date: 2020-08-24T02:50:32.733Z
draft: false
featured: false
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---

# Problem


Given an integer `n`, add a dot (".") as the thousands separator and return it in string format.



**Example 1:**

```
Input: n = 987
Output: "987"
```

**Example 2:**

```
Input: n = 1234
Output: "1.234"
```

**Example 3:**

```
Input: n = 123456789
Output: "123.456.789"
```

**Example 4:**

```
Input: n = 0
Output: "0"
```



**Constraints:**

* `0 <= n < 2^31`

``

` `
# Solution
### Python3
```
    a=str(input())
    l=[]

    t=len(a)%3
    if (t!=0):
        l.append(a[:1*t])

    for i in range(int(len(a)/3)):
            l.append(a[t+3*i:t+3*(i+1)])


    m=""
    c=0
    for j in l:
        c=c+1
        if (c<len(l)):
            p='.'
        else:
            p=''
        m=m+j+p
    return m


```