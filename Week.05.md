# 경상북도 시, 군을 대상으로 출생수 최댓값 구하는 프로그램
```py
import pandas as pd
'''
#데이터 업로드

file="d:\PM12.csv"

data=pd.read_csv(file, encoding="euc-kr")
#print("데이터 업로드 완료")

print("연별 경상북도 시, 군의 출생수")
print(data)

print("\n연별 출생수 최대값")
print(data.max(numeric_only=True))

print("\n연별 출생수 최소값")
print(data.min(numeric_only=True))
```

```py
a=200
b=300
temp = a
a=b
b=temp

print(f"두 수의 자리 교환 : a={a},b={b}")
```

```py
kor=[95,90]
eng=[85,80]

total_k=kor[0]+kor[1]
print(f"국어 점수 합계:{total_k}")

total_e=eng[0]+eng[1]
print(f"영어 점수 합계:{total_e}")
```

```py
a=1000
p=2000
m=3000

su1=int(input("사과 개수입력:"))
su2=int(input("배 개수입력:"))
su3=int(input("멜론 개수입력:"))

a_t=int(a*su1*0.9)
p_t=p*su2
m_t=m*su3

t=a_t+p_t+m_t
print(f"가격:{t}")
```

```py
apple=int(input("사과 개수를 입력 :"))
pear=int(input("배 개수를 입력 :"))
melon=int(input("배 개수를 입력 :"))

fruit=[1000,2000,3000]

apple_t=int(apple*fruit[0]*0.9)
pear_t=pear*fruit[1]
melon_t=melon*fruit[2]
total=apple_t+pear_t+melon_t

print(f"가격:{total}")
```

# 딕셔너리 형태
```py
fruit={
    "apple":1000,
    "pear":2000,
    "melon":3000}

total=0

for f_name, pay in fruit.items():
    count=int(input(f"구입할 {f_name}의 갯수 입력:"))

    if f_name=="apple":
        pay=pay*0.9
        
    total=int(total+(count*pay))

print(f"총 지불액:{total}")
```
