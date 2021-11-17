# Java-study
자바 개념 정리 
<br><br>

## Contents
- [자바 프로그래밍](#자바-프로그래밍)
- [변수와 자료형](#변수와-자료형)
- [연산자](#연산자)
- [조건문과 반복문](#조건문과-반복문)
- [](#)
- [](#)
<br><br>

## 자바 프로그래밍

<details>
<summary><b>프로그래밍이란?</b></summary>

- 프로그래밍: 컴퓨터가 일을 수행하도록 프로그래밍 언어로 명령어 집합(프로그램)을 만드는 일
- 컴파일: 프로그래밍 언어를 컴퓨터가 실행가능한 기계어로 만드는 일
- 컴파일러: 기계어로 바꾸어 주는 프로그램 (ex. 자바 컴파일러, gcc)
</details>

<details>
<summary><b>자바 프로그래밍</b></summary>

- 자바의 역사
    - 1991년 제임스 고슬링을 비롯한 선 마이크로 시스템스 연구원들이 처음 개발
    - 가전, 휴대용 장치에 사용되는 소프트웨어 언어로 개발됨
    - 안정성이 중요
- 자바 프로그래밍의 특징
    - 플랫폼에 영향을 받지 않으므로 다양한 환경에서 사용할 수 있음   
    ![1-1](https://user-images.githubusercontent.com/84164109/138914154-f9a1716a-5415-45b9-b2ca-17da1c08ba94.png)
    - 객체 지향 언어이기 때문에 유지보수가 쉽고 확장성이 좋음
    - 프로그램이 안정적임
    - 풍부한 기능이 제공되는 오픈 소스
</details>

<details>
<summary><b>객체 지향 프로그래밍이란?</b></summary>

- 프로그램의 구현을 시간의 흐름순이 아닌 객체간의 관계와 협력을 기반으로 프로그램하는 것
- Object Oriented Programming(OOP) 이라고 함 (cf. 절차 지향 프로그래밍(Procedural Programming))
- 사용하는 언어: Java, C++, C#, Python, JavaScript, Ruby 등 다수 
- 장점: 재사용성, 유지보수, 코드 관리, 신뢰성 높은 프로그램
</details>
<br>

## 변수와 자료형

<details>
<summary><b>컴퓨터에서 자료 표현하기</b></summary>

- 2진수
    - 0과 1로만 데이터를 저장함
    - bit(비트): 컴퓨터가 표현하는 데이터의 최소 단위로 2진수 하나의 값을 저장할 수 있는 메모리의 크기
    - byte(바이트): 1byte = 8bit
- 2진수와 10진수   
    ![2-1](https://user-images.githubusercontent.com/84164109/138914139-205f0e98-d2dd-4872-9a23-6903468b4ba2.png)
- 2진수와 8진수, 16진수   
    ![2-2](https://user-images.githubusercontent.com/84164109/138914131-f936fc1a-6633-47b8-8f07-473fb590428c.png)
</details>

<details>
<summary><b>변수(Variable)</b></summary>

- 변수의 사용
    - 프로그램에서는 항상 변하는 값을 나타낼 필요가 있음 (ex. 학생의 성적, 합계, 게임의 레벨, 회원 주소 등)
    - 표현하려는 수에 맞는 데이터 타입(자료형)을 이용하여 변수 선언
    - 표현하려는 자료가 숫자, 문자, 문자열 등 다양할 수 있으므로 그에 맞는 자료형 사용
    - 변수 선언은 자료형과 변수 명으로 선언하며 선언과 동시에 초기화할 수 있음
- 변수의 이름
    - 영문자(대문자, 소문자)와 숫자, 특수문자 중 $, _ 사용 가능 (ex. count100, _master)
    - 시작은 숫자로 할 수 없음 (ex. 27days (X), 1abc(X))
    - 자바에서 이미 사용하고 있는 예약어는 사용할 수 없음 (ex. while, break 등)
    - 변수 이름은 프로그램 내에서 사용되는 것이므로 그 용도에 맞고 가독성이 좋게 만드는 것이 중요함
</details>

<details>
<summary><b>변수와 메모리</b></summary>

- 변수를 선언하면 해당되는 자료형의 크기만큼 메모리 할당
- 변수는 할당된 메모리를 가리키는 이름
</details>

<details>
<summary><b>기본 자료형(privitive data type)</b></summary>

![3-1](https://user-images.githubusercontent.com/84164109/138914113-6096025c-fbf8-4179-b6d3-69e997af9f2a.png)
</details>

<details>
<summary><b>정수형</b></summary>

![3-4](https://user-images.githubusercontent.com/84164109/138916452-bfecdab6-8000-4cc4-afc1-e1020b9214b7.png)

- byte와 short
    - byte: 1바이트 단위의 자료형으로 동영상, 음악 파익, 실행 파일의 자료를 처리할 때 사용
    - short: 2바이트 단위의 자료형으로 C/C++ 언어와 호환 시 사용
- int   
    ![3-4 - 복사본](https://user-images.githubusercontent.com/84164109/138916500-899bafa2-c707-4cf8-b180-3f3fe66964ae.png)
    - 자바에서 사용하는 정수에 대한 기본 자료형
    - 4바이트 단위의 자료형
    - 프로그램에서 사용하는 모든 숫자(리터럴)은 int로 저장됨
    - 32비트를 초과하는 숫자는 long 자료형으로 처리
- long
    - 8바이트 단위의 자료형
    - 숫자의 뒤에 알파벳 L 또는 l을 써서 long형임을 표시   
    (ex. int num = 12345678900; // error
        long lnum = 12345678900; // error
        long lnumber = 12345678900L; // ok)
</details>

<details>
<summary><b>실수형</b></summary>

- 부동 소수점 방식
    - 실수는 정수보다 정밀하기 때문에 정수와는 다른 방식으로 표현해야 함   
    (ex. 부동 소수점 방식으로 실수 값 0.1 표현)   
    ![3-3](https://user-images.githubusercontent.com/84164109/138914256-576a8b4f-2ffb-4387-a428-ae8104ca5939.png)
    - 지수부와 가수부로 표현
    - 컴퓨터에서는 밑수를 2로 사용
    - 정규화: 가수가 밑수보다 작은 한 자리까지 기수로 표현되는 것
    - 컴퓨터에서는 밑수가 2이므로 정규화를 하게 되면 가수부분의 첫번째 자리 숫자는 항상 1이 됨 (ex. 0.2 = 0.4*2^(-1) = 1.6*2^(-3))
    - 지수부가 0을 표현할 수 없기 때문에 약간의 오차가 발생할 수 있음
- float와 double   
    ![3-5](https://user-images.githubusercontent.com/84164109/138914339-01cca55d-a0f9-48a9-81ed-6bf430b0a604.png)
    - 자바에서는 실수의 기본 타입으로 double을 사용
</details>

<details>
<summary><b>문자형</b></summary>

- 프로그램에서 문자의 표현
    - 문자도 정수로 표현함
    - 어떤 문자를 컴퓨터 내부에서 표현하기 위해 특정 정수값을 정의
    - 문자세트(character set): 각 문자를 얼마로 표현할 것인지 코드 값을 모아둔 것 (ex. ASKII, euc-kr, utf-8, utf-16 등)   
    ![3-6](https://user-images.githubusercontent.com/84164109/138914362-4a2fff26-f908-43dd-af94-3c1de39c31c1.png)

- 자바에서 문자의 표현
    - 자바는 문자를 나타내기 위해 전세계 표준인 UNICODE를 사용
    - utf-16 인코딩 사용 (모든 문자를 2바이트로 표시)

- char
    - 문자를 위한 데이터 타입
    - 내부적으로 숫자로 표현되므로 숫자를 넣어도 문자가 출력될 수 있음

- 참고
    - character set: 문자를 숫자로 변환한 값의 세트
    - encoding: 문자가 숫자로 변환되는 것
    - decoding: 숫자에서 다시 문자로 변환되는 것
    - ASKII code: 알파벳과 숫자 특수 문자등을 1바이트에 표현하는데 사용하는 문자세트
    - UNICODE: 전 세계 표준으로 만든 문자 세트
    - UTF-8: 1바이트에서 4바이트까지 다양하게 문자를 표현할 수 있음
    - UTF-16: 2바이트로 문자를 표현
    - [한글 유니코드 표](http://www.unicode.org/charts/PDF/UAC00.pdf)
</details>

<details>
<summary><b>논리형</b></summary>

- boolean
    - true(참), false(거짓) 두 가지만 나타냄
    - 1바이트 사용
    - 값이 존재하는지, 배열이 비었는지, 결과가 참인지 거짓인지 등을 표현
</details>

<details>
<summary><b>자료형 없이 지역변수 사용하기 (자바 10 지원)</b></summary>

- var
    - local variable type infernce
    - 추론 가능한 변수에 대한 자료형을 선언하지 않음
    - 한번 선언하여 추론된 변수는 다른 타입의 값을 대입할 수 없음
    - 지역 변수만 사용 가능
</details>

<details>
<summary><b>상수(constant)</b></summary>

- 변하지 않는 수 (ex. 원주율 = 3.14, 1년 = 12개월 등)
- final 예약어를 사용하여 선언
- 상수를 사용하면 변하지 않는 값을 반복하여 사용할 때 의미있는 문자로 인식하기 쉽고, 변하더라도 선언한 부분만 변경하면 되므로 여러 부분을 수정할 필요가 없음
</details>

<details>
<summary><b>리터럴(literal)</b></summary>

- 프로그램에서 사용하는 숫자, 문자, 논리값을 뜻함
- 상수 풀(constant pool)에 있음
- 정수 리터럴은 int로, 실수 리터럴은 double로 저장됨 (정수의 범위가 넘어가는 경우는 L, l을, float로 사용하려는 경우는 F, f 식별자를 적어야 함)
</details>

<details>
<summary><b>형 변환(type conversion)</b></summary>

- 서로 다른 자료형 간에 연산 등의 수행을 위해 하나의 자료형으로 통일하는 것
- 묵시적 형 변환(explicit type conversion, 자동 형 변환)과 명시적 형 변환(implicit type conversion, 강제 형 변환)이 있음
- 바이트 크기가 작은 자료형에서 큰 자료형으로의 형 변환은 자동으로 이루어짐
- 덜 정밀한 자료형에서 더 정밀한 자료형으로의 형 변환은 자동으로 이루어짐
    
![3-7](https://user-images.githubusercontent.com/84164109/138914404-9e7c8f1d-b75e-4c85-98b9-88b85e5d58d4.png)
</details>
<br>

## 연산자

<details>
<summary><b>항과 연산자</b></summary>

- 항(operand): 연산에 사용되는 값
- 연산자(operator): 항을 이용하여 연산하는 기호
</details>

<details>
<summary><b>대입 연산자(assignment operator)</b></summary>

- 변수에 다른 변수나 값을 대입하는 연산자
- 이항 연산자 중 우선 순위가 가장 낮은 연산자
- 왼쪽 변수(또는 식, 값) = 오른쪽 변수(또는 식, 값)
</details>

<details>
<summary><b>부호 연산자</b></summary>

- 단항 연산자
- 변수의 부호를 유지 하거나(+) 바꿈(-)
- 실제 변수의 부호가 변하려면 대입 연산자를 사용해야 함
</details>

<details>
<summary><b>산술 연산자</b></summary>

![3-8](https://user-images.githubusercontent.com/84164109/138914422-87c94c8f-419a-4295-9482-82032a0361b5.png)
- 사칙연산자
- %: 숫자 n 의 나머지 범위는 0 ~ n-1
</details>

<details>
<summary><b>복합 대입 연산자</b></summary>

- 대입 연산자와 다른 연산자가 함께 쓰임
    
![3-9](https://user-images.githubusercontent.com/84164109/138914439-f6607b47-f98d-446d-8619-30f86eae1417.png)
</details>

<details>
<summary><b>증가, 감소 연산자</b></summary>

- 단항 연산자
- 변수의 값을 1 더하거나 1 뺄 때 사용
- 연산자가 항의 앞에 있는가 뒤에 있는가에 따라 연산 시점과 결과가 달라짐
- 문장(statement)의 끝(;)을 기준으로 연산 시점을 생각해야 함
    
![3-10](https://user-images.githubusercontent.com/84164109/138914071-849d3db3-5f76-41c5-96aa-d821eb976ea9.png)
</details>

<details>
<summary><b>관계 연산자</b></summary>

- 이항 연산자
- 연산의 결과가 true(참), false(거짓)으로 반환 됨, 비교연산자 라고도 함
- 조건문, 반복문의 조건식으로 많이 사용 됨
    
![3-11](https://user-images.githubusercontent.com/84164109/138914036-27a72e0c-9c04-4357-a4b8-505b00d35aa9.png)
</details>

<details>
<summary><b>논리 연산자</b></summary>

- 관계 연산자와 혼합하여 많이 사용됨
- 연산의 결과가 true(참), false(거짓)으로 반환됨
    
![3-12](https://user-images.githubusercontent.com/84164109/138914015-28cd3b37-34c9-4d72-b72a-ee9d845ec56e.png)

- 단락 회로 평가(short circuit evaluation): 논리 연산에서 모든 항이 실행되지 않는 경우
    - 논리 곱(&&)은 두 항의 결과가 모두 true일 때만 결과가 true   
    -> 앞의 항의 결과가 false이면 뒤 항의 결과를 평가하지 않음
    - 논리 합(||)은 두 항의 결과가 모두 false일 때만 결과가 false   
    -> 앞의 항의 결과가 true이면 뒤 항의 결과를 평가하지 않음
</details>

<details>
<summary><b>조건 연산자</b></summary>

- 삼항 연산자
- 조건식의 결과가 true(참)인 경우와 false(거짓)인 경우에 따라 다른 결과가 수행됨
- if (조건문)을 간단히 표현할 때 사용할 수 있음
    
![3-13](https://user-images.githubusercontent.com/84164109/138914004-3bc1dd07-7afd-4fa0-80d7-b9c2ed4f2bd9.png)
</details>

<details>
<summary><b>비트 연산자</b></summary>

- 대입 연산자와 다른 연산자가 함께 쓰임
- 마스크: 특정 비트를 가리고 몇 개의 비트 값만 사용할 때
- 비트 켜기: 특정 비트들만을 1로 설정해서 사용하고 싶을 때
(ex. & 00001111 (하위 4비트 중 1인 비트만 꺼내기))
- 비트 끄기: 특정 비트들만을 0으로 설정해서 사용하고 싶을 때
(ex. | 11110000 (하위 4비트 중 0 인 비트만 0으로 만들기))
- 비트 토글:  모든 비트들을 0은 1로, 1은 0으로 바꾸고 싶을 때
    
![3-14](https://user-images.githubusercontent.com/84164109/138913983-3f248bb7-b64e-46af-8175-a0398d4319d2.png)
</details>

<details>
<summary><b>연산자 우선순위</b></summary>

![3-15](https://user-images.githubusercontent.com/84164109/138913762-b9858343-b334-4b3b-ad39-2a773d7a9317.png)
</details>
<br>

## 조건문과 반복문

<details>
<summary><b>조건문이란?</b></summary>
주어진 조건에 따라 다른 실행이 이루어지도록 구현
</details>

<details>
<summary><b>if 문</b></summary>

``` java
if (조건식) {
    수행문;
}
```
</details>

<details>
<summary><b>if-else 문</b></summary>

``` java
if (조건식) {   
    수행문1;   
}   
else {   
    수행문2;   
}   
```
</details>

<details>
<summary><b>if-else if-else 문</b></summary>

``` java
if (조건식1) {   
    수행문1;   
}   
else if (조건식2) {   
    수행문2;   
}   
else if (조건식3) {   
    수행문3;   
}   
else {   
    수행문4;   
}   
```
</details>

<details>
<summary><b>if 문과 else if 문의 차이점</b></summary>

- if-else if를 사용하는 경우 하나의 조건이 만족되면 나머지 else if 부분은 수행되지 않음
- if-if로 사용하게 되면 각각 다른 조건문으로 해석되어 각각 수행하게 됨
</details>

<details>
<summary><b>switch-case 문</b></summary>

- if-else if-else 문을 사용할 때 복잡하고 번거로운 부분을 가독성 좋게 구현
- 비교 조건이 특정 값이나 문자열인 경우 사용
- break 문을 사용하여 각 조건이 만족되면 switch 블럭을 빠져나오도록 함
- 자바 14부터 좀 더 간결해진 표현식이 지원됨 (break 사용하지 않음)
``` java
switch (변수) {   
    case 조건1:   
        수행문;   
        break;   
    case 조건2, case 조건3:   
        수행문;   
        break;   
    default:   
        수행문;   
}   
```
</details>

<details>
<summary><b>while 문</b></summary>

- 수행문을 수행하기 전 조건을 체크하고 그 조건의 결과가 true인 동안 반복 수행
- 조건이 참(true)인 동안 반복수행하기
    - 주어진 조건에 맞는 동안(true) 지정된 수행문을 반복적으로 수행하는 제어문
    - 조건이 맞지 않으면 반복하던 수행을 멈추게 됨
    - 조건을 주로 반복 횟수나 값의 비교 결과에 따라 true, false 판단됨
``` java
while (조건식) {
    수행문1;
}
수행문2;
```
![1-1](https://user-images.githubusercontent.com/84164109/142200455-81a04d03-93c1-44f2-8915-b2855c78bb03.png)

- 무한 반복
``` java
while (true) {
    수행문;
}
```
</details>

<details>
<summary><b>do-while 문</b></summary>

- 조건과 상관없이 한번은 수행문을 수행
    - while 문은 조건을 먼저 체크하고 반복 수행이 된다면, do-while 문은 조건과 상관없이 수행을 한번 하고나서 조건을 체크
``` java
do {
    수행문1
} while (조건식);
수행문2;
```
![1-2](https://user-images.githubusercontent.com/84164109/142200488-6dd26cfe-0b50-413b-8a99-4ab5b827474e.png)

</details>

<details>
<summary><b>for 문</b></summary>

``` java
for (초기식; 조건식; 증감식) {
    수행문;
}
```
![1-3](https://user-images.githubusercontent.com/84164109/142200521-2a85c0d2-e1fe-4b36-814d-c67e78eed073.png)

</details>

<details>
<summary><b>for 문의 문장 생략</b></summary>

- 초기식 생략: 이미 이전에 값이 초기화되어 for 내부에서 값을 지정할 필요가 없는 경우   
``` java
int i = 0;
for (; i<5; i++) {
    ...
}
```
- 조건식 생략: 반복 수행에 대한 조건이 수행문 내부에 있는 경우   
``` java
for (i=0; ; i++) {
    sum += i;
    if (sum > 200) break;
}
```
- 증감식 생략: 증감식에 대한 연산이 복잡하거나 다른 변수의 연산 결과값에 의해 결정되는 경우   
``` java
for (i=0; i<5; ) {
    ...
    i = (++i)%10;
}
```
- 무한 반복
``` java
for (; ; ) {
    ...
}
```
</details>

<details>
<summary><b>각 반복문을 사용하는 경우</b></summary>

||while|do-while|for|
|-|-|-|-|
|수행|조건이 참인 동안 반복 수행<br>조건이 맞지 않으면 수행되는 부분이 없음|조건이 참인 동안 반복 수행<br>수행문을 먼저 수행하고 조건 체크|초기화, 조건 체크, 증감 순으로 진행|
|쓰임|조건식의 결과가 변수나 true, false 값인 경우 주로 사용|조건식의 결과가 변수나 true, false 값인 경우 주로 사용|특정 수의 범위, 횟수와 관련하여 반복되는 경우 주로 사용<br>배열과 함께 많이 사용|
</details>

<details>
<summary><b>중첩 반복문</b></summary>

- 반복문 내부에 또다른 반복문이 있음
- 여러 겹으로 반복문을 겹쳐서 구현 가능 (단, 수행시간에 문제가 발생할 수 있음)
- 외부 반복문과 내부 반복문 간의 변수 값 변화에 유의하며 구현해야 함
</details>

<details>
<summary><b>break 문과 continue 문</b></summary>

- break
    - 감싸고 있는 제어문의 블록을 빠져나오는 기능 (switch 문에서도 사용)
    - 반복문에서는 주로 조건문(if)와 같이 사용하며, 조건에 해당되는 경우 반복 수행을 멈추고 반복문 외부로 수행이 이동
    - 여러 반복문이 중첩되어 있는 경우, break 문이 포함되어 있는 반복문만 빠져나옴
- continue
    - 반복문 내부에서 조건문(if)와 같이 사용하며, 조건이 맞는 경우(true) 이후 반복문 블럭 내부의 다른 수행문들을 수행하지 않음
</details>
<br>
