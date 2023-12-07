# 모델링(Modeling)
* **모델을 만드는 작업**, 현실 세계(실체)를 단순화 시켜 표현하는 기법
* 현실을 간단하게 설명하기 위해 **여러 단위들 간의 관계도**로 보여주는 형태
<p align="center">
  <img src="https://github.com/jeong-vely0611/UML/assets/148931569/04203dc0-36fe-4cd7-9490-cfdb11b40a28" height="250px">
</p>


# UML (Unified Mdeling Language)
* **`통합 모델링 언어`** (소프트웨어 공학에서 사용되는 표준화된 모델링 언어) <br>
* 소프트웨어 개념을 **시각적으로 표현**하기 위해 사용하는 다이어그램(수식관계를 그림으로 표시) 표기법<br>

### 1. UML의 필요성
* **의사소통 하기 좋음** <br>
   : 가시화 시킴으로써 개발자와 고객사 간의 의사소통을 원활하게 도와줌
* **대규모 프로젝트 구조의 로드맵을 만들 때 유용함** <br>
   : 로드맵을 통해 개발자가 프로젝트 구조에 대해 빨리 파악할 수 있음
* **개발할 시크템 구출에 대해 기초를 마련할 수 있음** <br>
   : 구현하는 시간을 단축 할 수 있음
* **백엔드 문서용으로 적합함**

### 2. UML 작성(모델링) 시 주의사항
* 핵심적인 기능 위주로 간결하게 작업 (복잡하게 작업 X)
* 반복을 통해 수정 (분석/설계 단계에서만 하는것이 아니므로, 다듬어 나가는 것이 중요!)
* 모델링 후 다이어그램을 봤을 때 코드를 작성할 수 있어야 함

### 3. UML 다이어그램 종류
* 크게 **`정적 다이어그램`** 과 **`동적 다이어그램`** 으로 나뉨

<p align="center">
  <img src="https://github.com/jeong-vely0611/UML/assets/148931569/bea145ad-ef62-4928-9513-1db31a346f73" height="150px">
</p>

<p align="center">
  <img src="https://github.com/jeong-vely0611/UML/assets/148931569/30fdd619-1842-42a4-b0d7-11b65c126cdb" height="300px">
</p>

* **클래스 다이어그램** 
   : 프로그램 안의 주요 클래스와 관계를 나타낸 다이어그램
* **유스케이스 다이어그램** 
   : 시스템과 사용자의 상호작용을 나타내는 기능 위주의 다이어그램
* **시퀀스 다이어그램**
   : 시간 흐름에 따른 객체 사이의 상호작용을 나타낸 다이어그램

### 4. UML 툴 설치
> starUML 5.0 설치(UML 툴 중에서 가장 보편화 되어 있는 프로그램)

1. http://sourceforge.net/projects/staruml/files/staruml/5.0
2. Download Latest Version 클릭 후 exe 설치
3. Next > 경로 설정, Next > ...
4. 사용자 가이드 : http://staruml.sourceforge.net/docs/user-guide(ko)/toc.html
5. profile 설정하기(Tools > Java > Generate Code 클릭 시 오류 창 뜰 때)
   * Model > Profiles > Java Profile 선택 > Include > Close

### 6. V 프로세스 
<p align="center">
  <img src="https://github.com/jeong-vely0611/UML/assets/148931569/50d4db67-c9ff-468b-aa46-649273822d8d" height="250px">
</p>

* V프로세스(모델) 기법은 모델링 단게 뿐만 아니라 테스팅 단계에서도 많이 사용 됨
* 전체적인 흐름을 한눈에 파악하기 쉬움
* 양쪽이 서로 대칭이 되기 때문에 비교하기 좋음 (블랙박스 vs 화이트박스)
  * **블랙박스** : 사용자의 관점으로 분석하는 단계 (이용할 때의 기능을 분석)
  * **화이트박스** : 시스템 관점으로 분석하는 단계 (시스템 코드 구성 등 분석) 
  



