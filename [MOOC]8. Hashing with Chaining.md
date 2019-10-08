# 8. Hashing with Chaining

###  # Dictionary Type

=> Only Know about it's exist

( Key , value )



### # Motivation

- docdist
- database
- compilers & interpreters
- internet router
- substring search
- string commonalities



### # Badness

1. Key may not be integer
2. gigantic Memory hog



### in Python hash(x) is the prehash of X 



### # Chaining = 충돌의 해답법







## Q/A

* Dictionary가 사용될 수 없는 곳은 어떤 특징이 있나요?
  
  * 조합이 Key , Value 값으로 이루어 지지 않았다는 특징이 있다.
  
* Chaining 이외에 해시테이블에서 충돌이 일어날때 해결할 수 있는 방법이 있을까요?
  
  *  해당 부분의 배열을 복사하여서 몰아 넣을 수 있다.
  
* Chaining을 연결리스트 이외에 다른 방법으로 할 수 있는 방법은 없나요?

  * 2차원 배열에 희소행렬을 이용한다.

    

## Words



