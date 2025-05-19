```py
# 응용과제
print("내신 등급 계산 프로그램")

sub_k=int(input("내신 등급 계산할 과목 수 입력 : "))
sub_c=list(map(int,input("과목별 단위 수 입력(공백으로 구분하여 과목 수 만큼 입력) : ").split()))
sub_r=list(map(int,input("과목별 석차입력(공백으로 구분하여 과목 수 만큼 석차입력) : ").split()))

sum_r=sum(sub_c)
sum_k=0
for i in range(sub_k):
    sum_k+=(sub_c[i]*sub_r[i])

grade=round(sum_k/sum_r,1)

print(f"귀하의 내신 등급은 {grade}입니다.")
if (grade<=3):
    print("귀하의 내신 수준은 상위권")
elif(grade<=6):
    print("귀하의 내신 수준은 중위권")
else:
    print("귀하의 내신 수준은 하위권")
```

```py
# 실습 예제 4-6
pwrd=list(input("type in word :")) # list 굳이 안붙여도 되는듯

if (pwrd[0]=="a"):
    print("A")

else:
    print("not A")
```

```py
# 실습 예제 4-7
pwrd=input("Enter your password :")
if (len(pwrd)>=7):
    print("Save Success")
else:
    print("Save Fail")
```

```py
# 응용문제
pwrd=input("비밀번호 입력 (7자 이상의 문자로 시작하고, 첫글자는 반드시 대문자) :")
if (pwrd[0].isupper() and len(pwrd)>=7):
    print("비밀번호 설정 완료")
else:
    print("조건에 맞지 않음")
```

# 조건문 삼항 연산자
```py
a,b=map(int,input("두 수 입력:").split())
print(f"{a}가 더 큽니다")if(a>b)else print(f"{b}가 더 큽니다.")
```

### 연습문제
```py
h=int(input("심박수 :"))
t=float(input("체온 :"))
o=int(input("산소포화도 :"))
print("응급: 즉시 조치 필요")if(h<=40 or o<90) else print("경고: 의사 호출 필요") if(t>=39 or o<95) else print("정상 상태 유지")
```
