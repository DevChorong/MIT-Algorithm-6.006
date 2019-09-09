# Models of Computation, Document Distance

### # what Algorithm is

it's start by Al-Khwarizmi

[Informal Definition]

=> Computational Procedure for solving a problem

input -> algorithm -> output



### # Program vs Algorithm

| X      | Program              | Algorithm            |
| ------ | -------------------- | -------------------- |
| write  | Programming Language | Pseudocode           |
| Run in | Computer             | Model of Computation |

Computational Model specifies

* what operation an Algorithm is allowed
* Cost ( time complexity, space Complexity ) of each up



### # RAM

| Computer             | Model of Computation  |
| -------------------- | --------------------- |
| Random Access Memory | Random Access Machine |

### # The Theory side

* RAM in Computer 
  * Modeled by Big array
  * in Constant time can
    * load Constant<mark>(O(1))</mark> words
    * do constant Computations
    * store constant words
  * Have Constant registers
  * LOAD - COMPUTING - STORE
  * Word : w bits ( Size : Log(size of Memory) )
* Pointer Machine
  * Dynamically allocated objects
  * object has constant fields
  * field = words (eg. int)
  * field = pointer

### # The Python Side

in python We can do lot of things

<mark>The Point is "which one is getting more time"</mark>

* List = array
* object with constant attributes



### # Document distance problem 

#### d(D1, D2)

Document = Sequence of words

word = String of Alphanumaric chars

idea : shared words

think of document as a VECTOR

D[w] = count of w in D

### # Algorithm to solve this problem

> 1. Split document into words
> 2. compute word frequencies
> 3. dot product



### # Qs

* Q1. Computer에서 RAM은 Array로 구현된다. 그렇다면 계산 모델(Computatioal Model) 에서는 무엇으로 구현 될까?
  * A1. 물리적인 저장장소(예를 들면 종이문서 등)라고 생각한다. Computer에서의 RAM은 저장에 큰 의미를 두고 있고, 따라서 그 특징이 가장 큰  종이 문서등이 Computer에서의 Array를 대신해서 구현 가능 하다고 생각한다.



* Q2. RAM을 설명 할 때 "상수(Constant)"라는 말이 매우 자주 나온다. 그 이유에 대해서 생각나는 대로 적어보시오
  * A2. 왜냐하면 RAM이 PC에서의 Random Access Memory던 모델상의 Random Access Machine 이던 간에 물리적인 공간에서 물리적인 계산과 물리적인 저장으로 이루어져 있기 때문에 물리적인 한계인 상수로 표현이 가능 하기 때문이다.



* Q3. 시간 복잡도를 줄입에 있어서 가장 중요한 것은 무엇일까요?
  * A3. 그것은 바로 복잡도의 차수를 줄이는 것이라고 생각한다. 선형 시간이였던 것을 상수시간으로, 2차 시간이였던 것을 상수시간으로 줄이기 등 차수가 하나 올라갈 때 마다 복잡도는 배로 증가한다고 생각하기 때문에 차수를 줄여서 최소의 연산을 유도하는 것이라고 생각한다.  



* Q4. 시간 복잡도를 개선하는 것이 가장 큰 영향을 받는 것은 어느때 인가?
  - A4. 바로 Input의 크기가 커질 때이다. 시간복잡도의 차수를 줄이거나 복잡도를 줄여 나감은 시간이 배로 감소 된다고 생각한다. 따라서 Input의 크기에 따라 영향도 크게 보일 것으로 생각한다.



* Q5. 왜 이 강의에서 Document distance 를 구할때 단어(word)가 아니라 문서(Document)를 하나의 Vector로 보았는가?
  * A5. 왜냐하면 단어를 하나의 속성( feature, 다른말로 하나의 축 )으로 보기위해서 이다. 그렇게 되면 하나의 속성이 된 단어를 축으로 만들어서 같은 단어가 있다면 그축으로 기울어짐을 통해서 "두 문서가 유사함"에 가까워 질 수 있기 때문이다.



## Words

Computation : 계산

