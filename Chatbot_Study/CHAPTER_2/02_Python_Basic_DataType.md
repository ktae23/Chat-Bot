# 파이썬

## 2.1 파이썬 소개

> 파이썬은 전 세계적으로 가장 많이 사용하고 있는 언어 Top 3에 랭크 될 만큼 넓은 사용자 층을 보유하고 있는 언어입니다. 코드 수정 없이 다양한 플랫폼에서 사용 가능하며, 셀 수 없을 정도의 다양한 라이브러리를 보유하고 있어 인기가 좋습니다.
>
> 또한 머신러닝 및 데이터마이닝 관련 프레임워크에서 메인 언어로 사용하고 있기 때문에 챗봇 엔진 개발에 있어 필수  언어입니다.

<br/>

지난 주말에 카페에 갔을때 사람들의 노트북 속에서 파이썬 라이브러리를 활용한 데이터 시각화 화면을 심심찮게 볼 수 있었다. 

우리나라에서는 데이터 업계에서만 많이 쓰이고, 자바와 자바스크립트가 워낙 큰 영향을 가지고 있지만, 파이썬은 뭐랄까, 미워할 수 없는 막내 같다고 해야하나?

<br/> 어느샌가 옆자리를 차지하고 넓히는데 미워할 수 없는, 그런 언어 같다.

<br/>

파이썬 2버전은 공식 지원이 종료 되었고 최근에 나오는 머신러닝 프레임워크들도 3.x 버전을 기반으로 배포 되고 있다.

파이썬 3은 2버전과 달리 모든 변수를 객체로 처리하며, 모든 문자열을 유니코드인 str 객체로 통일 했다.

<br/>

## 2.2 파이썬 기본

> 일반적으로 프로그램 내부 코드는 동작 행위와 데이터 상태로 구분되어 있습니다. 여기서 동작 행위란 프로그래머가 정해놓은 순서나 의도대로 컴퓨터가 동작을 할 수 있도록 미리 함수나 메서드 형태로 정의해 놓은 것입니다.
>
> `중략`
>
> 이 절을 통해 파이썬에서는 함수와 데이터를 어떻게 사용하는지 알아볼 것입니다.

<br/>

### 2.2.1 자료형

> 자료형이란 프로그램 내부에서 사용하는 데이터의 형태를 의미합니다. 언어에 따라 데이터의 형태를 엄격하게 구분하기도 하지만 파이썬의 경우에는 조금 느슨한 편입니다.

<br/>

#### 숫자

##### 정수 계산

```python
>>> 10 + 5
15
>>> (10 - 5) * 2
10
>>> 10 // 2
5
```

- 파이썬에서는 소수점을 사용하지 않는 한 기본적으로 int형으로 처리 한다.
- 대화형 인터프리터를 기본 예제에 사용했기에 >>>(prompt)가 보인다.
  - 마치 스피드 퀴즈를 하듯이 연산 결과를 받을 수 있다.

<br />

##### 실수 계산

```python
>>> 2.2 * 5
11.0
>>> 1.0 / 0.2
5.0
>>> 3 / 2
1.5
```

- 파이썬에서 소수점을 사용하거나 기본적으로 계산 결과가 실수인 경우에는  float형으로 처리 한다.

- 그러고보니 라인 끝마다 `;` 를 안해도 된다니 편하다.
  - 처음에 파이썬부터 배웠어서 자바에서 `;` 빼먹는 경우가 많았는데, 어제는 글쓰다가 보니 문장 끝에 마침표 대신 세미콜론 찍고 있더라;;ㅋㅋ

<br/>

> 파이썬에서 나눈셈 `/`의 연산 결과는 항상 실수 형태인 float형이입니다.
>
> 나눗셈을 정수 형태로 얻기 위해서는 `//`을 사용해야 하며, 나머를 계산하기 위해서는 `%`연산자를 사용해야 합니다.

<br/>

---

<br/>

##### 거듭 제곱

```python
>>> 2 ** 5
32
>>> 2 ** 10
1024
```

> 챗봇 개발에 필요한 딥러닝이나 통계 모델을 구현할 경우 복잡한 수식을 사용해야 할 때가 있습니다.(복잡한 수식이라고 했지만 추상화가 많이 된 함수 형태로 사용하기 때문에 실제로는 복잡하지 않습니다.) 
>
> 그중에서 가장 많이 사용하는 연산자가 거듭제곱입니다. 파이썬에서 고듭제곱은 `**`로 표현합니다.

<br/>

##### 변수 입력

```python
>>> a = 10
>>> b = 20
>>> a * b
200
```

> 변수를 나타낼 때는 등호(=)를 사용합니다.
>
> 변수명은 숫자로 시작할 수 없으며, 특수 기호 및 시스템 키워드가 아니라면 어떤 형태로도 사용 가능하며, 개발 방법에 따라 명명 규칙이 정해져 있는 경우가 많습니다.

<br />

---

<br/>

#### 문자열

##### 문자열 구분

```python
>>> '1234'
'1234'
>>>  'hello'
'hello'
>>> "hello"
'hello'
```

> 문자들의 집합을 의미합니다. 사용자와 소통하는 프로그램에서 문자열 처리는 필수적이며, 프로그래밍 언어에 따라 사용 방법이나 난이도가 다를 수 있습니다.
>
> `중략`
>
> 파이썬은 큰따옴표나 작은따옴표를 이용하여 문자열을 표현합니다. 인터프리터는 문자열 결과를 보여줄 때 숫자값과 구분하기 위해 기본적으로 작은따옴표로 묶어서 출력합니다.(문자열에 작은따옴표가 포함 되어 있는 경우에는 큰 따옴표로 묶습니다.)

<br/>

##### 변수 입력

```python
>>> msg = 'Hello'
>>> msg
'Hello'
>>> error = "err 404"
>>> error
'err 404'
```

>  변수를 나타낼 때는 등호(=)를 사용하며, 큰따옴표나 작은따옴표를 사용해서 문자열이라고 표시해주면 됩니다.

<br/>

```python
>>> msg1 = '"Nice to meet you", chatbot says'
>>> msg1
'"Nice to meet you", chatbot says'
>>> msg2 = "I'm programming now"
>>> msg2
"I'm programming now"
```

> 문자열 내의 작은따옴표 출력을 위해서는 큰 따옴표로 묶고, 큰따옴표 출력을 위해서는 작은 따옴표로 묶습니다.

<br/>

##### 줄 바꿈

```python
>>> msg3 = 'Hell0\nbro!!'
>>> msg3
'Hell0\nbro!!'
>>> print(msg3)
Hell0
bro!!
```

- 줄 바꿈을 위해 이스케이프 코드 `\n`을 사용하였으나 그냥 변수를 출력하면 줄 바꿈이 안된다. 
  - print() 함수를 사용해 변수를 출력하면 적용 된다.

```python
>>> msg4 = '''Hello
... bro!!'''
>>> msg4
'Hello\nbro!!'
>>> print(msg4)
Hello
bro!!
```

- 간단한 문장일 경우 `\n`사용, 복잡한 문장일 경우 작은따옴표 세개 `'''` 또는 큰 따옴표 세개`"""`를 연속으로 사용한다.

> 이스케이프 코드
>
> | 이스케이프 코드 | 의미        |
> | --------------- | ----------- |
> | \n              | 줄 바꿈     |
> | \t              | 탭          |
> | \\              | 문자 \ 출력 |
> | \'              | 문자 ' 출력 |
> | \"              | 문자 " 출력 |

<br/>

---

<br/>

#### 리스트 

> 서로 관계가 있는 데이터들은 목록이나 집합 형태로 관리할 필요가 있습니다. 파이썬에서는 서로 다른 형의 데이터를 한꺼번에 묶을 수 있는 여러 가지 자료형을 제공합니다.
>
> 리스트는 대괄호 []를 사용하며, 데이터 요소들을 쉼표(,)로 구분합니다.
>
> 숫자, 문자열, 객체형 데이터도 추가 할 수 있습니다.
>
> 서로 다른 형의 데이터를 동시에 저장할 수 있지만 보통 같은 형의 데이터만 추가해서 사용합니다.

<br/>

```python
>>> numbers = [1,2,3,4,5]
>>> numbers
[1, 2, 3, 4, 5]
>>> real_numbers = [1.0, 2.0, 3.0, 4, 5]
>>> real_numbers
[1.0, 2.0, 3.0, 4, 5]
>>> type(real_numbers)
<class 'list'>
```

<br/>

- 리스트는 문자열과 마찬가지로 인덱싱과 슬라이싱 지원
- 인덱싱
  - 0부터 시작하며 인덱스 접근 시 [] 대괄호 사용
- 슬라이싱
  - [시작위치:끝 위치]를 사용해 새로운 리스트를 생성
  - 원본 리스트를 훼손하지 않은 채 슬라이싱 된 요소들이 새로운 리스트로 생성 됨

<br/>

```python
>>> numbers = [1,2,3,4,5]
>>> numbers[1]	# 1번째 요소 인덱싱(0부터 시작)
2
>>> numbers[-1]	# 뒤에서 1번째 
5
>>> numbers[2:]	# 2번째요소부터 끝까지 슬라이싱
[3, 4, 5]
>>> numbers[-2:]	# 뒤에서 두번째 요소부터 슬라이싱
[4, 5]
>>> numbers[1:-2]	# 1번째 요소부터 뒤에서 두번째까지 슬라이싱
[2, 3]
```

<br/>

##### 리스트 요소 수정

```python
>>> numbers = [1,2,3,4,5]
>>> numbers[0] = 9
>>> numbers
[9, 2, 3, 4, 5]
```

<br/>

##### 리스트 요소 추가

```python
>>> numbers = [1,2,3,4,5]
>>> numbers.append(9)
>>> numbers
[1, 2, 3, 4, 5, 9]
```

- 리스트.append(자료)
  - 자료를 리스트의 마지막 요소로 추가

<br/>

##### 리스트 요소 삽입

```python
>>> numbers = [1,2,3,4,5]
>>> numbers.insert(1, 1.5)
>>> numbers
[1, 1.5, 2, 3, 4, 5]
```

- 리스트.insert(인덱스 번호, 자료)
  - 자료를 인덱스 번호 위치에 삽입

<br/>

##### 리스트 삭제

```python
>>> numbers = [1,2,3,4,5]
>>> numbers.pop()
5	# 꺼낸 값이 출력 됨
>>> numbers
[1, 2, 3, 4]
#==============
>>> numbers = [1,2,3,4,5]
>>> numbers.pop(2)
3
>>> numbers
[1, 2, 4, 5]
```

- 리스트.pop(인덱스 번호)
  - 인덱스 번호 없으면 마지막 자료가 출력되고 삭제 
  - 인덱스 번호 있으면 해당 인덱스 위치 요소가 출력되고 삭제

<br/>

```python
>>> numbers = [1,2,3,4,5]
>>> del numbers[2]
>>> numbers
[1, 2, 4, 5]
```

- del 리스트[인덱스 번호]
  - 인덱스 번호 위치의 요소 출력하지 않고 바로 삭제

<br/>

##### 리스트 요소 개수 구하기

```python
>>> numbers = [1,2,3,4,5]
>>> len(numbers)
5
```

<br/>

---

<br/>

#### 튜플

> 튜플은 리스트와 마찬가지로 다양한 데이터를 집합 형태로 관리할 수 있지만 한 번 생성되면 순서와 내용을 정할 수 없습니다.
>
> 또한 리스트는 요소들을 대괄호 []로 둘러싸지만 튜플은 소괄호()로 둘러 쌉니다.

<br/>

- 리스트와 마찬가지로 저장되는 요소들의 자료형에 제한이 없음
- 튜플은 요소 변경 불가

```python
>>> numbers = (1,2,3,4,5)
>>> nubmers
(1, 2, 3, 4, 5)
>>> real_numbers = (1.0, 2.0, 3.0, 4, 5, 'six')
>>> real_numbers
(1.0, 2.0, 3.0, 4, 5, 'six')
>>> type(real_numbers)
<class 'tuple'>
```

<br/>

- 튜플은 리스트와 마찬가지로 인덱싱과 슬라이싱 지원
- 인덱싱
  - 0부터 시작하며 인덱스 접근 시 [] 대괄호 사용
- 슬라이싱
  - [시작위치:끝 위치]를 사용해 새로운 튜플을 생성
  - 원본 리스트를 훼손하지 않은 채 슬라이싱 된 요소들이 새로운 리스트로 생성 됨

<br/>

```python
>>> numbers = (1,2,3,4,5)
>>> numbers
(1, 2, 3, 4, 5)
>>> numbers[1]
2
>>> numbers[-1]
5
>>> numbers[2:]
(3, 4, 5)
>>> numbers[-2:]
(4, 5)
>>> numbers[1:-2]
(2, 3)
```

<br/>

##### 튜플 요소 수정 (불가)

```python
>>> numbers = (1,2,3,4,5)
>>> numbers[0] = 9
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'tuple' object does not support item assignment
```

<br/>

##### 튜플 요소 덧셈 연산

```python
>>> numbers = (1,2,3,4,5)
>>> new_numbers = numbers + (6,7)
>>> numbers
(1, 2, 3, 4, 5)
>>> new_numbers
(1, 2, 3, 4, 5, 6, 7)
```

- 덧셈 연산을 이용해 추가한 듯한 효과를 줄 수 있음
  - 튜플객체끼리만 가능
  - 두개 이상의 요소가 있어야 가능
  - 요소가 하나일 경우 (1, )과 같이 표현

<br/>

---

<br/>

#### 딕셔너리

> 딕셔너리는 key와 value를 한쌍으로 가지는 해시(hash) 형태의 자료형입니다.
>
> 순차적으로 데이터를 검색하지 않습니다. 해당하는 key에 맞는 value만 바로 확인 할 수 있습니다.
>
> 저장되어 있는 key를 순차적으로 탐색하는 방법도 있습니다.

<br/>

```python
>>> user1 = {'name':'홍길동', 'age':'30', 'email' : 'hong@hanbit.co.kr'}
>>> user1
{'name': '홍길동', 'age': '30', 'email': 'hong@hanbit.co.kr'}
>>> type(user1)
<class 'dict'>
```

<br/>

- key와 value가 한쌍으로, 콜론:으로 구분하고 중활호{}로 둘러 싸고 있다.
- 각각의 쌍은 쉼표(,)로 구분한다.
- key에는 숫자(정수,실수)와 문자열만 사용 가능
- value에는 데이터 형태 제한 없음

<br/>

#### 딕셔너리 문자열 키

```python
>>> dict1 = {'kei' : [100, 'hi', 4.5]}
>>> dict1['kei']	# key가 'kei'인 value 확인
[100, 'hi', 4.5]	# key가 'kei'인 value가 List형
>>> dict1['kei'][1]	# key가 'kei'인 value(List형)의 인덱스 1번 요소 확인 
'hi'
```

<br/>

#### 딕셔너리 데이터 쌍 추가

```python
>>> dict3 = {}	# 비어 있는 딕셔너리 생성
>>> dict3['a'] = 'A'	# key가 'a'인 value에 'A'를 저장
>>> dict3['b'] = 'B'	# key가 'b'인 value에 'B'를 저장
>>> dict3
{'a': 'A', 'b': 'B'}
```

```python
>>> dict3[3] = [1,2,3]	# key가 '3'인 value에 리스트 [1,2,3]을 저장
>>> dict3[4] = {'name': 'Kei', 'age': 35}	# key가 '4'인 value에 딕셔너리 {'name': 'Kei', 'age': 35}를 저장
>>> dict3
{'a': 'A', 'b': 'B', 3: [1,2,3], 4: {'name': 'Kei', 'age': 35}}
```

- 따로 함수가 존재하지 않으므로 원하는 key와 value를 저장
- value에 다양한 형태의 자료형을 추가 할 수 있음

<br/>

#### 딕셔너리 데이터 쌍 삭제, 전체 삭제

```python
>>> dict3 = {'a': 'A', 'b': 'B', 3: [1, 2, 3], 4: {'name': 'Kei', 'age': 35}}
>>> del dict3['a']	# key 값이 'a'인 데이터 쌍 삭제
>>> del dict3[3]	# key 값이 3인 데이터 쌍 삭제
>>> dict3.clear()	# dict3의 모든 데이터 쌍 삭제
>>> dict3
{}
```

<br/>

---

<br/>

#### 불리언

> 참(True)과 거짓(False)를 나타내는 자료형으로, 해당 조건이 참인지 거짓인지 논리적으로 판별하는 데 사용합니다. 간단하게 불(bool)자료형으로 불리기도 합니다.

```python
chek = True
uncheck = False
type(check)
<class 'bool'>
uncheck
False
```

- 첫 글자는 항상 대문자로 작성