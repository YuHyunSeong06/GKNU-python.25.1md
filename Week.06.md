# cm를 inch단위로 변환하는 코드
```py
num=int(input("Input cm:"))

inch=round(num/2.54,2)

print(f"transform inch :{inch} ")
```

# 반지름 r 값을 입력받아 원의 넓이를 구하는 코드
```py
pi=3.141592653589793238

r=int(input("Input r:"))

s=round(r**2*pi,3)

print(f"s={s}")
```

# random 함수를 이용하여 1~100까지 수를 n 만큼 구하기
```py
n=int(input("Input r:"))

for i in range (n):
    n2=randint(1,100)
    print(n2)
```

# 문자길이 구하기
```py
text="중간고사 화이팅"
print(f"{text}:{len(text)}")
```

# 리스트의 갯수 세기(len 함수)
```py
list_1=[1,2,3,4,5,6,7,8,9,10]
len_1=len(list_1)
print(f"리스트 요소의 갯수 : {len_1}")
```

# 1부터 10까지의 합계
```py
summ=sum(list_1)
print(f"1부터 10까지의 합 : {summ}")
```

# 정사각형이 원내부에 접해있을때 원의 면적 구하기
```py
a=int(input("a="))
s=round((sqrt(a**2+a**2)/2)**2*pi,2)
print(f"Circle Area:{s}")
```

