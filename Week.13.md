### 반복문 정리
~~

### 비밀번호 반복
```py
password=""
while password != "1234":
    password=input("비밀번호를 입력하세요:")
print("접속 성공!")
```
### 실습예제 5-1 - for
```py
total=0

for i in range(11):
    total+=1
print(f"for문:1부터 10까지 정수의 합 : {total}")
```

### 실습예제 5-1 - while
```py
x=int(input("반복할 수 입력 : "))
total=0
i=1
while(i<=x):
    total+=i
    i+=1

print(f"while문 : 1부터 10까지의 정수합 : {total}")
```

### 실습예제 5-1 - sum 
```py
total=sum(range(1,11))

print(f"sum함수 : 1부터 10까지 정수의 합 :{total}")
```
### 원금 100만원 복리 5% 10년 뒤 가치 프로그램 - for
```py
PV=1000000 # 현재 가치(원) : 초기 투자금
n=10 # 저축기간(년)
FV=PV # 미래 가치(원) : 초기 투자금으로 시작
r=5 # 이자율(%)

print(f"원금 : {FV:,.0f}. 이자 : {r}%")

for i in range(n):
    FV=FV+(FV*(r/100))
print(f"수령 예정 금액 : {FV:,.0f}원")
```

### 원금 100만원 복리 5% 10년 뒤 가치 프로그램 - while
```py
PV=1000000
n=10
FV=PV
r=5
i=1

print(f"원금 : {FV:,.0f}), 이자 : {r}%")

while (i<=n):
    FV=FV+(FV*(r/100))
    i+=1
    
print(f"수령 예정 금액 : {FV:,.0f}원")
```
### 원금 100만원 이자가 20% 복리일때 원금의 10배가 되는 년도
```py
PV=1000000
FV=PV
r=20
y=0

print(f"원금 : {FV:,.0f}, 이자 :{r}%")

while (FV<=PV*10):
    FV=FV+(FV*(r/100))
    y+=1

print(f"예상 저축 기간 {y}년")
```
### 두 주사위를 던져 합이 6이 되는 경우
```py
maxNum=6
cnt=0
a=1 # 첫번째 주사위
while (a<=maxNum):
    b=1 # 두번째 주사위
    while (b<=maxNum):
        if(a+b==6):
            cnt+=1
            break
        b+=1
    a+=1
print(f"2개의 주사위 합이 6이 되는 경우의 수 : {cnt}개")
```
