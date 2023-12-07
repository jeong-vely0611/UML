# 클래스 다이어그램
> **정적(구조) 다이어그램**으로, UML모델링에서 가장 많이 사용<br>
> **시스템의 구조와 구조 간 상호 관계**를 나타내며, 시스템의 논리적 및 물리적 구성요소 설계 시 주로 활용

### 1. 클래스의 표현
<p>
  <img src="https://github.com/jeong-vely0611/UML/assets/148931569/901fee2c-9baf-4fdc-bab1-fb4b99e4a448" height="200px">
</p>

* 클래스는 논리적 설계와 물리적 설계가 있음
* 첫 번째 칸은 클래스 명(이름)을 작성
* 가운데 칸은 속성과 자료형을 작성 (= **`멤버 변수`**)
* 마지막 칸은 연산과 자료형을 작성 (= **`메소드`**)

<br>

 ### 2. 접근 제한자
 |접근제한자|예약어|적용 범위|
 |:---:|:---:|:---:|
 |+|public|전체|
 |#|protected|같은 패키지 + 상속 관계|
 |~|default|같은 패키지|
 |-|private|같은 클래스|

<br>

 ### 3. 표기 방법
 |표현법|적용 범위|예약어|
 |:---:|:---:|:---:|
 | <u>attribute</u> , <u>method</u> (밑줄)|속성(변수), 연산(메소드)|static|
 |FIELD|속성(상수)|final|
 | *Class* , *method* (기울임)|클래스 명(추상 클래스), 연산(추상 메소드)|abstract|

<br>

 #### 4. 클래스 다이어그램 속성 및 활용법
 1. **`Add Model`** > **`Add Diagram`** > **`Class Diagram`**
 2. Class 만든 후, 속성과 연산(메소드) 추가    
    * **`Add Arribute`** (초록색) : [접근제한자]속성 및 자료형 작성
    * **`Add Operation`** (빨간색) : [접근제한자]연산 및 반환타입 작성
    <p>
      <img src="https://github.com/jeong-vely0611/UML/assets/148931569/704e356a-2845-49ac-b800-6f5b3dee051b">
    </p>
3. **`Visibility`** : 접근제한자 변경하기 
4. **`InitialValue`** : 값 초기화 하기 
5. **`OwnerScope`** : static 속성으로 변환하기  ->  CLASSIFIER
6. **`Changeability`** : 상수 선언하기(final, 값 변환되지 않게 하기) -> FROZEN
    <p>
      <img src="https://github.com/jeong-vely0611/UML/assets/148931569/1a4ce00c-d795-4ad9-8440-29486302b29c" height="180px">
    </p>    
7. **`IsAbstract`** : 추상 메소드로 변경하기 (추상메소드를 가지면 추상클래스이므로, 클래스도 IsAbstract로 추상클래스로 변환해 주어야 함)
    <p>
      <img src="https://github.com/jeong-vely0611/UML/assets/148931569/c258b339-9071-43ab-a867-3a0d63899f47" height="200px">
    </p> 
8. 자바(Java)의 소스코드 뽑아내기
   * 단, getter/setter 메소드는 직접 구현해야 함
    <p>
      <img src="https://github.com/jeong-vely0611/UML/assets/148931569/640a66a3-8601-43d6-b7f4-aa8b7bcc55e4" height="150px">
    </p> 

<br>

### 5. 클래스 다이어그램의 관계
<p>
  <img src="https://github.com/jeong-vely0611/UML/assets/148931569/42d5c42f-dae8-4170-b302-34ae1698cadc" height="300px">
</p>
