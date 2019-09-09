# Insertion Sort, Merge Sort

### # Why Sorting?

**The Point is Problem that become easy once items are sorted**

ex. Finding a median in unsorted array A[0 : n] -> B[0 : n]

-> if we have sorted array B we spend constant time

ex. in Binary search Looking for specific item

<mark>**Every Sorting Algorithms have reason that made**</mark>



### # First Sorting Algorithm :: Insertion Sort ( 삽입 정렬 )

* what is it?
  * For i = 1, 2, ... , n // Insert A[i] in to Sorted array A[ 0 : i-1 ] by pairwise swaps down to the correct position
* The Point?
  * Key( Pointer that move right side when Algorithm computing )
  * Pairwise Swap! ( exchange as Binary Search )
* Binary Search Insertion Sort?
  * Not good for Sort because it has Delta(n^2) time complexity
  * so find Delta(N log N)
* that so we think about Complexity
  * In recursive Binary Tree we can get C\*n -> C\*n/2 -> C\*n/4 -> ... -> C for in (1 + log n)
  * so T(n) = (C\*n) * (1 + log n) = Delta( n log n )



### # Second Sorting Algorithm :: Merge Sort ( 병합 정렬 )  

* Split array A to array L & array R

* and again and again and again and again....

* never Changing is **Merge Two Sorted array = Delta(n)**

* | # 1      | split array A to array L & array R ( they are unsorted) |
  | -------- | ------------------------------------------------------- |
  | **\# 2** | **define L' made by sorted L & R' made by sorted R**    |
  | **\# 3** | **Merge L' and R' to array A**                          |

### 

### # Recursive Tree ( 재귀 트리 )

* what is Recursive Tree



### # what Advantage Insertion Sort

* it's Sorted at in-place so Insertion Sort has not need any other Space to Sorting
* but the Merge Sort need to a Space to sort L'  & R'



### # way of This Class

- Normal Insertion Sort
- Binary Tree Insertion Sort ( Pairwise swap was exchanged by Binary Tree)
  - if (Compare >> swaps) use Binary Tree
  - then Delta(n^2) ----> Delta( n log n )
- Recursive Tree Insertion Sort ( Binary Tree was exchanged by  Recursive Tree)
- Merge Sort
- 3 Recursive Tree





## Q/A

* 버블 정렬과 삽입 정렬의 시간 복잡도 부분에서의 가장 큰 차이점은 무엇일까요?
  * 버블 정렬의 경우 고정적으로 '이차시간(n^2)' 이지만 삽입정렬의 경우 이미 정렬이 되어있는 경우에는 
    '선형시간(n)'이고 역순으로 되어있는 경우에는 '이차시간(n^2)'이므로 가변 적이라는 특징이 있는 것 같다.



* 정렬 알고리즘이 만들어진 것에는 다 이유가 있다고 했습니다. 그렇다면 정렬을 하면 좋은 문제와 정렬을 하면 오히려 안좋은 문제의 가장 큰 차이점은 무엇일까요?
  * 순서를 알아야 하거나 위치와 같은 "특정 부분"에 대한 정보를 원하는 경우에는 정렬을 하는 것이 좋다 하지만 "미래 예측"과 같이 주어진 데이터의 흐름을 보는 정보의 경우에는 정렬을 하는 것이 오히려 데이터를 쓸모 없도록 만들 수 도 있다. 따라서 가장 큰 차이점은 "특정"이냐 "전체"이냐 인 것 같다. 



* 삽입 정렬에서 재귀 트리를 사용하는 것과 사용하지 않는 것의 차이는 무엇인가요?
  * 시간 복잡도의 이득을 볼 수 있는가 없는가의 차이인 듯 하다.



* 병합 정렬에서 2개의 array 가아니라 더많은 양의 서브루트로 나누었을때의 시간복잡도가 더 작지 않을까??

  * ( 개인적인 생각 ) array 가 많아짐에 따라서 연산해야할 부분이 많아져서 시간 복잡도의 개선은 되지 않을 것 같다.

  

* 삽입 정렬에서 처음 시작 Key가 여러개가 되면 시간 복잡도가 개선 될 수 있지 않을까? (ex 3개 -> 2개 -> 1개)
  
  * (개인적인 생각 ) Key 가 많아지면 작업해야할 부분이 많아질 수 밖에 없고 또한 불필요하게 여러번의 작업이 반복적으로 일어나는 부분 ( 연산이 겹치는 부분 )이 있어서 시간 복잡도가 오히려 더 늘어날 것 같다. 다만, 겹치는 연산만 피한다면 오히려 더 빨라질 수 도 있을 것 같다.

## Words

recursive : 재귀적인

in-place :  제자리 

