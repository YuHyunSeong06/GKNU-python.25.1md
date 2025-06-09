### 한 병에 300원 우유 3병이 공병이면 새 우유 하나 줌. 24,300원으로 먹을 수 있는 우유의 개수
```py
price=int(input("한병의 가격을 입력하시오. : "))
money=int(input("현재 소지하고 있는 금액을 입력하시오 : "))

d_milk=money//price

print(f"첫 번째 우유병 수 :{d_milk}")

t_milk=d_milk

while(d_milk>=3):
    d_milk=d_milk//3
    t_milk=t_milk+d_milk
    print(f"공병으로 교환한 우유 수 : {d_milk}")


print("총",t_milk,"병의 우유를 마실 수 있다.")
```

### 원하는 단만 출력
```py
i=int(input("출력할 구구단 입력 :"))

for j in range (1,10):
    print(f"{i}x{j}={i*j:2}")
```

### 구구단 가로 출력
```py
print(" "*50,"구구단 출력\n")

for i in range(2,10):
    for j in range(1,10):
        print(f"{i} x {j} = {i*j:2}",end="   ")
    print()
```
