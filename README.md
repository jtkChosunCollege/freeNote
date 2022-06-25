# freeNote
그날 공부했던 부분들을 정리하여 올리는 repository입니다. 주로 readme.md 파일을 사용합니다.

# 2022년 Note 정리

## 6월

### 220625

파이썬 영상 보기 완료.

** 파이썬 기초 문법 첫걸음 1시간 반짜리. **

https://www.youtube.com/watch?v=M6kQTpIqpLs&t=324s


튜터님이 올려주신 Python 공부자료.
자료이름|자료주소|
---|---|
파이썬 기초 문법 첫걸음 1시간 반짜리.|https://youtu.be/M6kQTpIqpLs
점프 투 파이썬 | https://wikidocs.net/book/1
파이썬 300제 | https://wikidocs.net/book/922

파이썬 300제 023문제까지 해결했다.

### 220625

Q3

while문을 사용하여 다음과 같이 별(*)을 표시하는 프로그램을 작성해 보자.

```
*
**
***
****
*****
```

내가 작성한 코드

```python
a = 1
i=a
while a<6:
    while i!=0:
        print('*',end="")
        i-=1
    a+=1
    i=a
    print('')
```

Q4

for문을 사용해 1부터 100까지의 숫자를 출력해 보자.

내가 작성한 코드

```python
for a in range(1,101):
    print(a, end=' ')
```

Q5

A 학급에 총 10명의 학생이 있다. 이 학생들의 중간고사 점수는 다음과 같다.

[70, 60, 55, 75, 95, 90, 80, 80, 85, 100]

for문을 사용하여 A 학급의 평균 점수를 구해 보자.

내가 작성한 코드

```python
A = (70, 60, 55, 75, 95, 90, 80, 80, 85, 100)
total = 0
avr = 0
for i in A:
    total += i
avr = total/len(A)

print(avr)
```

Q6

리스트 중에서 홀수에만 2를 곱하여 저장하는 다음 코드가 있다.



```python
numbers = [1, 2, 3, 4, 5]
result = [] 
for n in numbers:
	if n % 2 == 1:
		result.append(n*2) 
```

위 코드를 리스트 내포(list comprehension)를 사용하여 표현해 보자.

내가 작성한 코드

``` python
numbers = [1, 2, 3, 4, 5]
result = [ n * 2 for n in numbers if n % 2 == 1 ]
print(result)
```



