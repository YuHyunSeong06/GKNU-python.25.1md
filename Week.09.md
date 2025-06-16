# 1차시
### 람다함수
```py
square = lambda x: x*x

print(square(5))
```

### 함수를 통한 두 수의 합
```
def add(a,b):
    c=a+b
    return c

ret = add(3,4)

print("숫자 1과 숫자 2의 합을 구하는 함수의 결과 값: ",ret)
```

### 더하기 함수
```
def add(a,b):
    return a+b #토글형

print(add(3,4)) #정수형
print(add(3.1,4.7)) #실수
print(add([1,2,3],[4,5,6])) #리스트형
print(add('Apple','Mango')) #문자형 
print(add(['rock'],['paper','scissors'])) #자료형
```

### 구구단 함수 버전
```
def gugudan(n):
    for i in range(1,10):
        res = n*i
        print(n,"X",i,"=",res)

while True:
    n=int(input("출력할 단 입력: "))
    if n==0:
        print("안녕")
        break
    gugudan(n)
```

# 2차시
### 약수 구하는 함수
```
def getDivisors(n):
    res=[]
    for i in range(1,n//2):
        if n%i==0:
            res.append(i)
    return res

print(getDivisors(28))
```

### 함수를 사용한 크기 비교
```
def max_value(a,b):
    if a>b:
        print(a,"가 더 크다")
    elif a<b:
        print(b,"가 더 크다")
    else:
        print(a,"와 ",b,"는 크기가 같다")
        
    
for i in range(5):
    a=int(input("숫자1 입력: "))
    b=int(input("숫자2 입력: "))

    max_value(a,b)

#max_value(10,20)
```

# 3차시
### bmi지수 계산
```
def bmi(we,hi):
    bm=we/(hi*hi)

    if bm<18.5:
        print("저체중")
    elif 18.5<=bm and bm<=25: #교수님께서는 18.5>=bm으로 작성하셨으나 부등호 방향이 반대임
        print("정상")
    else:
        print("과체중")
for i in range(3):
    we=int(input("체중을 입력하세요(kg): "))
    hi=float(input("키를 입력하세요(m): "))
    bmi(we,hi)
```

### 함수 리턴을 사용한 계산
```
def circle_area(r):
    area1=3.14*r*r
    return area1

def rect_area(w,h):
    area2=w*h
    return area2

for i in range(3):
    r=int(input("원의 반지름 입력: "))
    area1=circle_area(r)
    print("원의 면적은? ", area1)

    w=int(input("가로면적 입력: "))
    h=int(input("세로면적 입력: "))
    area2=rect_area(w,h)
    print("사각형의 면적은? ", area2)
```

# 4차시
### 사칙연산
```
def plus(a,b):
    c=a+b
    print("더하기 결과: ",c)
    
def minus(a,b):
    c=a-b
    print("빼기 결과: ",c)
    
def multiply(a,b):
    c=a*b
    print("곱하기 결과: ",c)
    
def divide(a,b):
    c=a/b
    print("나누기 결과: ",c)

for i in range(3):
    a=int(input("첫번째 수 입력(a): "))
    b=int(input("두번째 수 입력(b): "))

    plus(a,b)
    minus(a,b)
    multiply(a,b)
    divide(a,b)
```

### 기말고사 평균을 입력받아 최대값과 최소값을 출력해주는 프로그램
```py
def max_jumsu(lst):
    return max(lst)

def min_jumsu(lst):
    return min(lst)

lst=[100, 90, 50, 60, 40, 80, 95, 20, 85, 15, 65]

result1=max_jumsu(lst)
result2=min_jumsu(lst)

print("기말고사 평균 점수 중 최고 점수: %d" %result1)
print("기말고사 평균 점수 중 최저 점수: %d" %result2)
```



