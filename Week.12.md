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
