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
