### Part 1

- namedtuple
  파이썬 2.6 부터 namedtuple 을 이용해서 데이터베이스의 레코드처럼 메서드를 가지지 않는 일련의 속성으로 구성된 클래스를 만들 수 있다.

  ```python
  import collections

  Card = collections.namedtuple('Card', ['rank', 'suit'])

  ranks = [1,2,3,4,5,6,7,8,9,10,11,12,13]
  suits = ['spade' 'diamond', 'clova', 'heart']

  cards = [Card(r, s) for s in suits for r in ranks]

  cards[0] # Card(rank=1, suit='spade')
  ```
