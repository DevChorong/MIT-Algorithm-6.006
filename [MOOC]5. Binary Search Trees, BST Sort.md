# 5. Binary Search Trees, BST Sort

### # Binary Search Tree (분할 정복법)



### # Scheduling Problem - Runway Reservation System

####  situation

> 1. Airport with a Single runway
> 2. Reservations for Future landing
> 3. Reserve request specific landing time 't'
> 4. add t to the set 'R' if no other landings are scheduled within 'k' min
> 5. remove from set R after airplane lands
> 6. all this processing time is O(log n)

 

### # Binary Tree

> * Parent
> * left child node ( key(y) <= key(x) )
> * right child node (key(y) >= key(x) )



### # Binary Tree complexity = O(h)



### #NEW Requirement : Rank(t) 

=> how many planes are scheduled to land at times <= t



> 1. add new number related in "size"
> 2. Add 1 to every node you see while passing by. (지나가는 동안 보이는 모든 노드에게 1을 더해준다.)



### # 한쪽으로 쏠린 트리는 결국 리스트의 형태를 갖게 된다.



## Q/A

* k와 이진트리는 무슨 상관 관계를 갖는가?
  * 기본적인 이진트리에는 삽입에 제약을 갖지 않는다. 다만 k를 넣어준 이유는 시간과 시간사이에 조건을 넣어준 것 뿐이다.
* 이 문제를 해결할 때 이진탐색트리를 사용하는 것이 가장 합리적인 본인이 생각하는 이유는 무엇인가??
  * 왜냐하면 이진 탐색트리는 한가지 노드를 중심으로 2개의 경우의 수만을 남겨둔다 (크거나 or 작거나) 따라서 노드를 삽입 시키는 시간 복잡도 면에서 큰 이득을 볼 수 있다고 생각한다.
* 기존에 문제에 새로운 문제를 추가할 때 시간 복잡도 면에서 O(h)를 유지할 수 있을까?
  * 유지할 수 있을 것이라고 생각한다. 어떤 문제가 오던간에 결국 이진트리 안에서 일어나는 모든 것이고, 형태를 변형 하지 않는 이상 삽입, 삭제, 변형 안에서 모든 문제가 일어날 것이라고 보기 때문이다.



## Words



