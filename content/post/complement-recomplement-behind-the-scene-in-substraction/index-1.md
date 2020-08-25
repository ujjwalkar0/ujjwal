---
title: "Behind the scene in substraction : Complement & Recomplement "
date: 2020-08-25T12:45:41.822Z
draft: false
featured: false
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---
## **10's complement :**

> **M-N when      M>N** 

 **9-3 = 6  --> is it correct ?**

**How to do substraction using complement ?**

**Step 1 :** 3 -----> \[ 10's complement ] ---->  10-3 = 7

**Step 2 :** 9+7 = 16   \[ 10's complement of answer ]

**Step 3 :** 16-10 = 6  \[ Recomplement ] \[ Final Answer ]

**Behind the scene !!**

**Step 1 :** (10 - 3) \[ 10's complement ]

**Step 2 :** 9 + 7 = 9 + (10 - 3) = (9 - 3) +10  \[ 10's complement of answer ]

**Step 3 :** (9-3) + 10  - 10 = (9-3) \[ Recomplement ] ---> which is the final answer.

> **M-N when M<N**

**3-9 = - 6 ----> Is it correct ?**

**Lets do this using complement.** 

**Step 1 :** 9 ----> \[ 10's complement ]  ---> (10-9) = 1

**Step 2 :** 3+1 = 4 \[ 10's complement of answer ]

**Step 3 :** 4 - 10 = -6 \[ Recomplement ] \[ Final Answer ]

**Behind the scene**

**Step 1 :** (10 - 9 ) \[ 10's Complement ]

**Step 2 :** 3 + 1 = 3 + (10 - 9 ) = (3 - 9) + 10 \[ 10's complement of answer ]

**Step 3 :** (3 - 9) + 10 - 10 \[ Recomplement ] = (3 - 9) \[ Final Answer ]

## **1's complement :**

> **M-N when      M>N**

**1101 - 1001 = 0100  ---->  is it correct ?**

**How to do substraction using complement ?**

**Step 1 :** 1001 ---> \[ 1's complement ]  ----> 1111 - 1001 = 0110

**Step 2 :** 1101 + 0110 = 10011

**Step 3 :** Remove extra carry 1 and add 1 to remaining digits. i.e.  0011 + 1 = 0100

**Behind the scene !!**

**Step 1 :** (1111 - 1001) \[ 1's Complement ]

**Step 2 :** 1101 + (1111 - 1001) = 1101 - 1001 + 1111

**Step 3 :** (1101 - 1001) + (1111 + 1 ) - 10000

> **M-N when      M<N**

**1001 - 1101 =  -0100 ---->  is it correct ?**

**How to do substraction using complement ?**

**Step 1 :** 1101 ---> \[ 1's complement ]  ----> 1111 - 1101 = 0010

**Step 2 :** 1001 + 0010 = 1011

**Step 3 :** Take complement with a minus sign, i.e. -0100

**Behind the scene !!**

**Step 1 :** (1111 - 1101) \[ 1's Complement ]

**Step 2 :** 1001 + (1111 - 1101) = 1001 - 1101 + 1111

**Step 3 :** 1111 - {(1101 - 1001) + 1111 }  \[ Recomplement ] = - (1101 - 1001)



## **2's complement :**

> **M-N when      M>N**

**1101 - 1001 = 0100  ---->  is it correct ?**

**How to do substraction using complement ?**

**Step 1 :** 1001 ---> \[ 1's complement ]  ----> 1111 - 1001 = 0110

**Step 2 :** 0110 + 1 = 0111 \[ 2's complement ] 

**Step 3 :** 1101 + 0111 = 10100

**Step 4 :** 10100 - 10000 = 0100

**Behind the scene !!**

**Step 1 :** (1111 - 1001) \[ 1's Complement ]

**Step 2 : (**1111 - 1001) + 1 \[ 2's complement ] 

**Step 3 :** 1101 + (1111 - 1001) + 1 = 1101 - 1001 + 1111 + 1

**Step 4 :** (1101 - 1001) + (1111 + 1 ) - 10000   //( As 1111 + 1 = 10000 )

> **M-N when      M<N**

**1001 - 1101 = - 0100  ---->  is it correct ?**

**How to do substraction using complement ?**

**Step 1 :** 1101 ---> \[ 1's complement ]  ----> 1111 - 1101 = 0010

**Step 2 :** 0010 + 1 = 0011 \[ 2's complement ]

**Step 3 :** 1001 + 0011 = 1100

**Step 4 :** Take 2's complement of 1100 , i.e. 0100 , and put a negative sign before result , i.e. -0100

**Behind the scene !!**

**Step 1 :** (1111 - 1101) \[ 1's Complement ]

**Step 2 :**  (1111 - 1101) + 1 \[ 2's Complement ]

**Step 2 :** 1001 + (1111 - 1101) + 1 = 1001 - 1101 + 1111 + 1

**Step 3 :** 10000 - {(1101 - 1001) + 1111+1 }  \[ Recomplement ] = - (1101 - 1001)