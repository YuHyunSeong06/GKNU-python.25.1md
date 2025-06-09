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

### 구구단 가로 출력 응용 - 열방향
```py
print(" "*50,"구구단 출력\n")

for i in range(1,10):
    for j in range(2,10):
        print(f"{j} x {i} = {i*j:2}",end="   ")
    print()
```

### 1부터 100까지 정수 중 3의 배수를 더하되 250을 넘는 순간 중지
```py
limits=250
total=0
times=0

for i in range(1,101):
    if(total<limits):
        if(i%3==0):
            total=total+i
            times+=1
       
            
            print(f"현재 값 : {i:>2}, 누적횟수 : {times:>2}, 합 : {total:>3} ")
```

### 10의 배수 10개를 원소로 갖는 배열 array를 만들고 출력
```py
arr=[10*i for i in range(11)]
print(f"배열요소 10개:{arr}")
```
# 터틀 그래픽 함수
### 사각형 그리기
```py
from turtle import *

s=Screen()
s.setup(400,400)
speed(3)
pensize(5)
shape("turtle")
color("blue")

penup()
goto(-50,-50)
pendown()

# 사각형 그리기
for i in range(4):
    forward(100)
    left(90)

s.exitonclick()
```

### 오각형 그리기
```py
from turtle import *

s=Screen()
s.setup(400,400)
speed(3)
pensize(5)
shape("turtle")
color("blue")

penup()
goto(-50,-50)
pendown()

# 오각형 그리기
for i in range(5):
    forward(100) # 100 단위 앞으로 이동
    left(72)     # 오른쪽으로 72도 회전 (360/5)
s.exitonclick()  # 클릭 시에 창 닫기
```

### 원 그리기
```py
from turtle import *

s=Screen()
s.setup(400,400)
speed(3)
pensize(5)
shape("turtle")
color("blue")

penup()
goto(-50,-50)
pendown()

# 원 그리기
circle(50)
penup()
forward(100)
pendown()
color("orange")
circle(50)
s.exitonclick()
```

### 오륜기 그리기
```py
from turtle import *

s=Screen()
s.setup(400,400)
speed(3)
pensize(5)
shape("turtle")
color("blue")

penup()
goto(-50,-50)
pendown()

# 각원의 펜 색상과 시작 위치를 설정합니다.
colors = ['blue','black','red','yellow','green']
positions = [(-110,0),(0,0),(110,0),(-55,-55),(55,-55)]

for i in range(5):
    pencolor(colors[i])
    #fillcolor(colors[i])
    penup()
    goto(positions[i])
    pendown()
    #begin_fill()
    circle(50)
    #end_fill()

hideturtle()
s.exitonclick()
```
