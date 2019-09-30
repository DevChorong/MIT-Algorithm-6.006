# 7. Counting Sort, Radix Sort, Lower Bounds for Sorting

### # Comparison Model

> * searching model : omega( log n )
> * sorting model : omega( n log n)



| decision tree      | algorithm               |
| ------------------ | ----------------------- |
| internal node      | binary decision         |
| leaf               | answer                  |
| root-to-leaf path  | algorithm execution     |
| path length(depth) | running time            |
| height of tree     | worst-case running time |



### # proof

<mark>Decision Tree is binary & must have >= n leaves one for each answer</mark>

=> Decision Tree's depth = log n



## O(n) Sorting algorithm

### # K가 적당할때

counting sorting( 계수 정렬 ) 을 쓴다. = O( n + k )시간

### # K의 크기에 상관없이

Radix Sorting ( 기수 정렬 )을 쓴다. = O( n log n)



## Q/A

* 결정트리를 이용 할 때 이진이 아닌 여러개의 연결된 노드를 사용하면 더 빠르지 않을까?
  * 조건이 다양해지는 만큼 더 시간이 걸릴 듯 하다.
* 알고리즘의 시간을 구할때 상한보다 하한을 구한 이유는 무엇일까?
  * 작업의 효율을 위해 최소 시간에 맞추어서 작성해야한다고 생각한다.

* 결정트리가 이진트리 뿐만 아니라 어느 알고리즘에 사용 될 수 있을까?
  * 병합정렬등 조건이 붙는 어느 알고리즘이라면 다 사용할 수 있다고 생각한다.

## Words



