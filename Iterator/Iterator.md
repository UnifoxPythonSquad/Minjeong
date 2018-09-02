Iterator
========

1.Iterator란 ?
---------------

* 반복 가능한 객체이며 반복문을 사용해 데이터를 순회하며 처리하는 것이다.
* 파이썬에서 반복자는 리스트, 튜플 등의 여러 개의 요소를 가지는 컨테이너에서 
 각 요소를 하나씩 꺼내 간편한 방법을 제공하는 객체이다.

**예제 1**
    >>> a = [1, 2, 3, 4]
    >>> a_iter = iter(a)
    >>> type(a_iter)
    <class 'list_iterator'>
    
    >>> next(a_iter)
    1
    >>> next(a_iter)
    2
    >>> next(a_iter)
    3
    >>> next(a_iter)
    4
    >>> next(a_iter)
    Traceback (most recent call last):
      File "<stdin>", line 1, in <module>
    StopIteration

**예제 2**
    >>> for element in [1, 2, 3]:
    ...     print(element)
    ...
    1
    2
    3

**예제 3**
    >>> for element in (1, 2, 3):
    ...     print(element)
    ...
    1
    2
    3
  
**예제 4**
    >>> for element in {1, 2, 3}:
    ...     print(element)
    ...
    1
    2
    3
    
**예제 5**
    >>> for key in {"a":1,"b":2,"c":3}:
    ...     print(key)
    ...
    a
    b
    c
    
**예제 6**
    >>> for char in "123":
    ...     print(char)
    ...
    1
    2
    3
    
**예제 7**
    >>> s = 'abc'
    >>> it = iter(s)
    >>> it
    <str_iterator object at 0x035027D0>
    >>>
    >>> next(it)
    'a'
    >>> next(it)
    'b'
    >>> next(it)
    'c'
    >>> next(it)
    Traceback (most recent call last):
      File "<stdin>", line 1, in <module>
    StopIteration
