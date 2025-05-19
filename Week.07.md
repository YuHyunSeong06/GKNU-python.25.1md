# 초를 입력받아 시:분:초 로 출력하기
```py
from math import *
from random import *

sec=int(input("Input second:"))

hour=int(sec/3600)
na=fmod(sec,3600)
minute=int(na/60)
second=int(fmod(na,60))

print(f"{hour}H {minute}M {second}S")
```

# 돈을 입력받고 동전으로 바꾸기
```py
from math import *
from random import *
 
cash=int(input("Send your money:"))
five_=int(cash/500)
na1=fmod(cash,500)
one_=int(na1/100)
na2=fmod(one_,100)
five=int(na2/50)
na3=fmod(na2,50)
ten=int(na3/10)
one=int(fmod(na3,10))

print(f"Get cash : 500*{five_} 100*{one_} 50*{five} 10*{ten} 1*{one}")
```

# 주사위를 굴려 이긴사람 정하기
```py
from math import *
from random import *


a=int(input("Rolling~ 1 to 6    "))
b=randint(1,6)

if a>b:
    print(f"A={a} B={b} A win!!!")

elif a==b:
    print(f"A={a} B={b} Draw...")

else:
    print(f"A={a} B={b} B win!!!")
```
