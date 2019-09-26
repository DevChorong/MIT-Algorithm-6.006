# 6. AVL Trees, AVL Sort

### #  height of a Node

-> length of longest path from it down to a leaf



more{ height( left child ), height( right child ) } + 1



### # AVL Tree

Require height of left & right children of every node to differ by at most |1|

| hl - hr | <= 1



### # 점화식 : N(h)= 1 + N(h-1) + N(h-2)

N(h) = 트리의 높이에 따른 노드의 수



### # AVL insert

> 1. simple BST insert



### # Rotation

> 1. left .Rotate()
> 2. right .Rotate()





## Q/A

* Q1. 트리에서 균형이 필요한 이유는 무엇인가요?
  * A1.  시간을 줄이기 위해서 라고 생각합니다. 서치를 할때 반으로 나눠야 하는데 시간을 조금 더 줄이려면 한쪽으로 치우쳐 있는 것 보단 반으로 나누어져 있어야 더 짧게 걸리기 때문입니다. 

*  Q2. 이진트리에서 노드의 수 와 높이중 균형에 있어서 더 중요한 것은 무엇일 까요?
  * A2. 물론 둘다 중요하지만 높이가 더 중요하다고 본다. 노드의 수가 아무리 많아도 높이가 낮으면 연산 횟수가 더 줄어들 기 때문이다.
* Q3.  트리의 균형을 위한 더 좋은 방법이 있을까?
  * A3. 새로운 노드를 삽입한다면 삽입한 후에 새로운 트리로 옮기는 방법을 시도해 보아도 좋을 것 같다.
* 

## Words



