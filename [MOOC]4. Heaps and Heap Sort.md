# Heaps and Heap Sort

### # Priority Queue ( 우선순위 큐 )

=> Implements a set S of elements, each of element associated with a key

**Insert(S , x ) : insert element x into set S**

**max(s) : return element of S with the largest Key**

**extract-max(s) : max(s)'' and remove it from s**

**Increase key(S, x, k) : Increase the value of x's key to new value k**



### # Heap

An array visualized an a nearly complete binary tree (완전 이진 트리 not 포화 이진 트리)

#### <mark>Heap on a Tree</mark>

> * Root of Tree : Fisrt element ( i = 1)
> * parent( i ) : i / 2
> * left( i ) : 2i
> * right ( i ) = 2i + 1

#### # Max-Heap property

: the key of a node is >= the key's of it's children ( 키값의 크기는 자식노드의 키값보다 크거나 같다. )



### # Min-Heap property

: the key of a node is <= the key's of it's children ( 키값의 크기는 자식노드의 키값보다 작거나 같다. )



### # Heap Operations

* build_max_heap()
  * Produces a max heap from a unordered array
* max_heapify()
  * correct **a single Violation** of the heap property in a subtree's root



### # max_heapify( A, i ) : 최대-힙 화

Assame that the trees rooted at left(i) and right(i) are max-heaps



### # Convert A[1 ... n] into a max-heap

Build_max_heap( A ) : 

​	for (i = n/2) down to 1

​		do max_heapigy( A, i )



### [Tips] A [ n/2+1 ,,, n ] : 단말노드



### # Heap Sort

> 1. Build_max_heap from unordered array [ O(n) ]
> 2. find max element A[1]
> 3. Swap elements A[n] with A[1]
>    now max element is at the end of array
> 4. DIscend node n from heap decrementing heap
> 5. new root may  violate max-heap but children are max_heaps_max_heapify



## Q/A

* 왜 min-heap이 아니라 Max-heap으로 정렬하는가?
  * max-heap에서는 가장 큰 값이 루트 노드에 해당 하게 된다. 따라서 max-heap을 이용해서 힙 정렬을 할때 큰값을 먼저 배치시켜 오름차순을 정렬하기 위해서 Max-heap을 사용한다고 생각한다. 반대로 내림 차순을 사용한다면 min-heap을 사용할 수 있다고 본다.
* 우선순위 큐를 만드는데 있어서 heap이 선택받은 이유는 무엇인가?
  * 힙은 큰값이 부모노드, 작은값이 자식노드 라는 구조를 가지고있어서 빠르게 큰값과 작은 값을 찾아낼 수 있기 때문이라고 생각한다.
* 힙정렬함에 있어서 왜 완전이진트리인가? 힙 구조의 특성상 큰값이 부모노드, 작은 값이 자식 노드라는 구조이다 그렇다면 완전이진트리가 아닌 일반적인 이진트리여도 구조의 특성을 갖는다면 사용할 수 있지 않을까?
  * 인덱스 번호 때문이라고 생각한다. 배열에 순서대로 넣는다고 가정한다면 힙을 정렬하는 Max-heapify의 실행(연산)부분을 보면 결국 인덱스 번호가 빠질 수 없다. 그래서 build-max-heap 과정도 있는 것이라고 생각한다.



## Words

ADT : 추상 자료형

