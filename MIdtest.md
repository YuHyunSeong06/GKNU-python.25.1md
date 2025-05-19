```py
from random import *
 
#실기 2(random 라이브러리의 함수를 활용하여 임의 수 출력, for문 내 코드 작성 제출)

i=0
for i in range(6):
    user=int(input("수 입력 (1에서 6사이에 수) :"))
    com=int(randint(1,6))

    if user+com==6:
        print(f"사용자 입력 수 : {user}, 컴퓨터 수 : {com} => 빙고")

    else:
        print(f"사용자 입력 수 : {user}, 컴퓨터 수 : {com}")
    

```
