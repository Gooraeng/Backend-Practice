# SQL 학습 공간
* [w3school](https://www.w3schools.com/sql/default.asp) 이나 [SQLBolt](https://sqlbolt.com/)를 통해서 SQL 언어에 따른 데이터를 가져오거나 변경하는 등의 변화 보기! 
* 2025년 5월 안에 프로그래머스 SQL LV1 완파 목표까지! 

## 관계형 데이터베이스 (Relational Database)?
* 엑셀처럼 행과 열의 2치원의 관계로써 표현되는 데이터베이스

### 예시)출석부

|학과|학년|학번|이름|
|---|---|---|---|
|전기|1|4|학생1|
|컴퓨터공학|3|5|학생2|
|화학|2|6|학생3|

#### 릴레이션 (= 테이블)
* 각 개체는 단일 값을 가진다. 
* 각 열의 순서는 없고, 유일하다. (학생부에 3학년 3학년 2반 같은 게 말이 안 되는 것처럼)
* 각 행의 순서는 없고, 문자로서 나타나는 값이 같더라도 그 성질이 다르다. (1학년 5반 김코딩, 3학년 4반 김코딩 같은 동명이인처럼)

#### 요소
* 열(= 필드, 속성) : 테이블의 한 열
* 행(= 튜플, 레코드) : 테이블의 한 행
* 도메인 : 한 필드에서의 값의 집합 (학년의 도메인 : 1, 2, 3)
* 키 : 각 튜플들을 구분하기 위한 것. (학번처럼 하나의 요소를 확실히 구분할 수 있는 것을 삼는 편)
  * 기본키 : 하나의 튜플을 구분하게 하는 고유한 키. 빈 값이 될 수 없고, 중복을 허용하지 않음.
  * 외래키 : 데이터가 일관될 수 있도록 돕는 것. 기본키와 보통 같이 사용되고, 둘 이상의 테이블을 연결하는 일종의 다리와도 같은 역할.

## SQL이란?
* 관계형 데이터베이스에 주로 사용되고, 이로부터 데이터를 추출하거나 변경, 삭제하도록 디자인된 언어.