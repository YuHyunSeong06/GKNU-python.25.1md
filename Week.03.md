# 평균계산 후 판단 프로그램
```python
x=int(input("put your write score : "))
y=int(input("put your active score : "))

avg=(x+y)//2

if avg>=90:
    print(f"average:{avg}, PASS")
else:
    print(f"average:{avg}, Sorry")
```

# 홀수 짝수 판단 프로그램
```python
x=int(input("Put num : "))
y=x%2

if y==0:
    print(f"{x}:even")
    
else:
    print(f"{x}:odd")
```

# 0부터 n까지 더하는 프로그램
```python
n=int(input("Put num : "))
sum=0
for count in range(n+1):
    sum+=count
print(f"1 to {n} total is {sum}")
```
# 입력한 숫자가 양수, 0, 음수인지 구분하는 프로그램
```python
n=int(input("Put num : "))
if n==0:
    print("n=0")

elif n>0:
    print("n is positive")

else:
    print("n is negative")
```
# 0에서부터 시작하여 입력한 숫자까지의 홀수만을 출력하는 프로그램
```python
n=int(input("Put num : "))
for count in range(0,n+1):
    if count%2!=0:
        print(f"{count}")
```
