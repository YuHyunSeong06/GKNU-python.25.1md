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
