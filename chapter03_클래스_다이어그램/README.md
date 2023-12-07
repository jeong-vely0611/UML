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

#### 5-1. 연관 관계
> 한 클래스가 **`필드`** 로 **다른 클래스를 참조할 때를 의미** <br>
> 클래스 간의 관련성을 뜻하는 것으로 **메시지 전달의 통로 역할**을 함

* **방향성이 없는 연관 관계** <br>
  : 쌍방향의 관계로, 각 클래스의 필드부에 상대 클래스를 참조하고 있음 (일반 실선으로 그려짐)
  <p>
    <img src="https://github.com/jeong-vely0611/UML/assets/148931569/b2f32d7f-5eb2-44d4-a73e-d56c954a860d">
  </p>
  
* **방향성이 있는 연관 관계** <br>
  : 방향성은 메세지 전달의 반향을 뜻하며, 반대 방향은 불가능 함 (한 쪽만 참조하고 있음)
    <p>
      <img src="https://github.com/jeong-vely0611/UML/assets/148931569/95d398bc-1664-4210-87be-823e218d2c83">
    </p>

* **연관 관계의 다중성** <br>
  : 관계를 맺을 수 있는 실제 상대 객체 수를 다중성을 동해 지정할 수 있음 (= 복수 개의 객체와의 관계) 
    <p>
      <img src="https://github.com/jeong-vely0611/UML/assets/148931569/950a8c32-5dec-4820-92d2-3e3578a7e715">
    </p>
    
* **다중 연관** <br>
  : 동일한 클래스 간의 존재하는 복수 개의 연관 관계를 뜻 함
    <p>
      <img src="https://github.com/jeong-vely0611/UML/assets/148931569/baf5168e-ef4d-40a4-b1dc-72fc5423f9f0">
    </p>

#### 5-2. 집합 관계
#### 5-3. 합성 관계
#### 5-4. 일반화 관계
#### 5-5. 실체화(인터페이스 실현) 관계 
#### 5-6. 의존 관계
#### 5-7. 인터페이스 의존 관계


