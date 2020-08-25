---
title: "Complement & Recomplement : Behind the scene in substraction"
date: 2020-08-25T06:49:42.984Z
draft: false
featured: false
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---
## **About 10's complement :**

> **M-N when      M>N**

 **9-3 = 6  --> is it correct ?**

**How to do substraction using complement ?**

3 -----> \[ 10's complement ] ---->  10-3 = 7

9+7 = 16   \[ 10's complement of answer ]

16-10 = 6  \[ Recomplement ] \[ Final Answer ]

**Behind the scene !!**

9 + 7 = 9 + (10 - 3) = (9 - 3) +10  \[ 10's complement of answer ]

or, (9-3) + 10  - 10 = (9-3) \[ Recomplement ] ---> which is the final answer.

> **M-N when M<N**

**3-9 = - 6 ----> Is it correct ?**

**Lets do this using complement.** 

9 ----> \[ 10's complement ]  ---> (10-9) = 1

3+1 = 4 \[ 10's complement of answer ]

4 - 10 = -6 \[ Recomplement ] \[ Final Answer ]

**Behind the scene**

3 + 1 = 3 + (10 - 9 ) = (3 - 9) + 10 \[ 10's complement of answer ]