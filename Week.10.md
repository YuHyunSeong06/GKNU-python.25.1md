```py
# 실습예제 4-1
ki=int(input("Your height : "))

if ki<100 or ki>200:
    print("Sorry to you can't ride this")

else:
    print("Have a nice time")
```

```py
# 실습예제 4-2
gen=input("Your gender male or female : ")
age=int(input("Your age : "))
if gen=="male" and age>=30 and age<40 :
    print("Test subject")
else:
    print("PASS")
```

```py
# 실습예제 4-3
name=input("Name : ")
t_num=int(input("Test number : "))
score=int(input("Score : "))
print(f"Name : {name}")
print(f"Test number : {t_num}")
if score>=70:
    print("Congratulation!!! you pass")
else:
    print("Sorry about that")
```

```py
# 실습예제 4-4 upgrade
w,p,a=map(int,input("Put score of 3 test : ").split())
if w>=90 and p>=90 and a>=90:
    print("Elite")
elif w>=60 and w and p>=60 and a>=60:
    print("Complete")
else:
    print("Re")
```

```py
# 실습예제 4-5 upgrade(배열로 정의)
a=list(map(int,input("Put 3 number : ").split()))
print(a)

if a[0]>a[1] and a[0]>a[2]:
    print(f"{a[0]} is biggest")
elif a[1]>a[0] and a[1]>a[2]:
    print(f"{a[1]} is biggest")
else:
    print(f"{a[2]} is biggest")
```
