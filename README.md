# stack

stack은  LIFO(Last In First Out) 구조로 차곡차곡 쌓아올렸다가 뺄때는 마지막에 넣은 놈 부터 빼는 것을 이야기한다. 

대표적으로 PUSH,POP, TOP등의 operator가 있다.

이는 linked list와 array로 구현하는 것이 일반적인데, 각각 장단점이 있다

## array로 구현시 장단점 : 

장점: 원하는 index에 접근해서 데이터 접근

단점: 배열의 size를 정의할때 fixed된 size를 정의해야하기 때문에 메모리 관리차원에서 비효율적 + 중간에 있는 데이터 삭제시 불편

## linked list 로 구현시 장단점:

장점: 원하는 위치에 데이터 삽입 및 삭제 용이(포인트 링크만 바꿔주면 되니까), 메모리 관리 효율적

단점: 그만큼 느림

## 용도:

대표적으로 인터넷에서 뒤로가기 등에서 사용되며 postfix연산, backtracking 등에서도 사용된다. 뿐만아니라 merge sort 등에서 사용되는 recursion을 구현할 때 스택이 사용된다.

## 문제풀이 10828번 :
```python
stack = []
stack.append(data)
print(stack.pop())
```

## 라이브러리? :

파이썬에서는 queue 모듈을 사용하면 된다. queue를 사용하여 stack 을 구현하는 것이 이상하긴 하지만 후입선출 큐 라는 의미로 LifoQueue 라는 녀석을 사용하면 stack을 사용할 수 있게 된다.

```python
s = queue.LifoQueue() 
```
