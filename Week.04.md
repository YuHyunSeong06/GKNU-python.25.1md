```python
msg = 'Welcome to Seoul'
print(msg.split(' '))
```

```python
str1='Welcome'
str3='Seoul'

print(str1 + str3)
```

```python
a,b,c,d,=12,56,23,41

x=(c+d)//(b+1)-a

print(x)
```

```python
print('a+b =',int(input('a='))+int(input('b=')))
```

```python
x=[23,14,25,17]
y=x[0]+x[3]
print(y)
```

```python
hob1=['reading','love','like']
print(hob1[1])
```

```python
animals=['lion','tiger','rabbit']

print(animals[0:1])

print(animals[1:2])

print(animals[1:3])
```

```python
a,b,c,d=2,5,10,20

x=(c+d)//(b+1)-a

print(x)
```

# pandas 활용
```python
import pandas as pd

#데이터 업로드

file="d:\PM10.csv"

data=pd.read_csv(file, encoding="euc-kr")
#print("데이터 업로드 완료")

print("월별 미세먼지 데이터")
print(data)

#월별 미세먼지 최대값
print("\n월별 미세먼지 최대값")
print(data.max(numeric_only=True))

#월별 미세먼지 최소값
print("\n월별 미세먼지 최소값")
print(data.min(numeric_only=True))
```
