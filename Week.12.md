### "vip" 20% 할인 "regular" 10% 할인
```py
value=int(input("결제 금액 입력 : "))
grade=input("고객등급입력 : ")
print(f"최종결제금액 : {int(value*0.8)}원") if(grade=="vip") else print(f"최종결제금액 : {int(value*0.9)}원")if(grade=="regular") else print(f"최종결제금액 : {int(value)}원")
```
### version 2
```py
value, grade = int(input("결제 금액 입력 : ")), input("고객등급입력 : ")
f_value = int(value*(0.8 if grade == "vip" else 0.9 if grade == "regular" else 1))
print(f"최종결제금액 : {f_value:,}원")
```

### in 을 사용한 조건 검사
```py
fruit=["apple", "banana", "cherrry"]
m_fruit="banana"
print(f"{m_fruit}는 목록에 있습니다.") if m_fruit in fruit else print(f"{m_fruit}는 목록에 없습니다.")
```

### in을 사용한 조건검사 연습문제
```py
name_l=["김지영","홍길동","강숙희"]
name=input("출석한 학생이름 입력 : ")
print("출석되었습니다.") if name in name_l else print("출석되지 않았습니다.")
```

### not을 사용한 조건 검사
```py
value=input("숫자를 입력하세요 : ")
print("숫자")if value.isdigit() else print("문자")
```

### if not 을 이용한 연습문제
```py
data=["admin","1234"]

id=input("아이디를 입력하세요 : ")
pwrd=input("비밀번호를 입력하세요 : ")
print("로그인 실패") if not (id==data[0] and pwrd==data[1]) else print("로그인 성공")
```

### 끝말잇기 게임
```py
word1=input("첫 번째 단어 : ")
word2=input("두 번째 단어 : ")
if word1[len(word1)-1]==word2[0]:
    print("끝말잇기 성공!!")
else :
    print("끝말잇기 실패..")
```

### 수행과제 4-4
##### 태어난 연도를 입력받아 윤년인지 아닌지 판별 프로그램
```py
for i in range(10):
    year=int(input("태어난 연도: "))
    print("윤년") if (year%4==0 and year%100 !=0 or year%400==0) else print("윤년 아님")
    if year==0:
        break
```

### 분리수거
```py
paper=["신문", "휴지", "책", "과자봉지"]
plastic=["락앤락","커피용기","페트병"]
can=["음료캔", "통조림"]
glass=["우유병", "콜라병"]

t_name=input("분류할 쓰레기의 이름을 입력하세요 : ")
print("종이류") if t_name in paper else print("플라스틱")if t_name in plastic else print("캔") if t_name in can else print("유리")
```

### 4-13
```py
age=int(input("나이를 입력하시오 : "))
time=int(input("입장시각(24)을 입력하시오 : "))
cash=20000
n_cash=15000

if(age>17 and age<65 and time<17):
    print(f"{cash}원")
elif(age>17 and age<65 and time>17):
    print(f"{n_cash}원")
elif(age>=7 and age<=17 and time<17):
    print(f"{cash*0.8}원")
elif(age>=7 and age<=17 and time>17):
    print(f"{n_casch*0.8}원")
else:
    print("입장료는 무료입니다")
```

### 연습문제 7번
```py
year=int(input("몇년도에 태어났나요? "))
ddi=["원숭이","닭","개","돼지","쥐","소","범","토끼","용","뱀","말","양"]
print(f"{ddi[int(year%12)]}")
```
