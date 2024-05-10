## 1. BST Performance
---
### Big O and Θ
Example: [[lec17_1.png]] [[lec17_2.png]]
## 2. Big O ≠ Worst Case
---
==Problem==: The shape of tree is decided only by the input order.
Worst and best example: [[20240510192627.png]]
==Solu==: In real worldm, using Randomize BST, which perform good both in add and delete method.
But, R-BST must have all data first. 
So... Let's creat efficient one.
## 3. 2-3-4 and 2-3 Tree Operations (a.k.a. B-Trees)
---
==Solu==: Overstuff
==Better==: 
1. Set a limit L on the number of items
2. Moving Items Up
3. Node Splitting

Example: [[20240510194532.png]] [[20240510195655.png]]
Perfect balance: [[20240510195906.png]]
## 4. B-Tree Bushiness Invariants
---
==My thought:== 
1. As for BST, we can create a new BST when a new item added in, with limitation like when height is too high or something.
2. BT is a good choice, splitting is creat a new one with a small move, and the limitation is L.
3. All methods should be efficient. Like add/delete/find. BT.find need to be compared with L items each nodes, which is not so fast as cut-half.

==Why==: BT always bushy?
These invariants guarantee that our trees will be bushy: [[20240510202405.png]]
## 5. B-Tree Performance
---
Runtime: O(log N).
Summery: [[20240510203929.png]]