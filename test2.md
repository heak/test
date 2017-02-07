## 2강

# 스키마

-데이터베이스를 구성하는 개체(entities),속성(attributes),관계(relations),및 데이터 조작(mainpulation) 시 데이터 값들이 갖는 제약조건(constraint)등에 관해 전반적으로 정의 

-스키마는 데이터 사전에 저장되며,다른 이름으로 메타 데이터라고도 한다.

-Schema is a collection of meta-data 

스키마는 메타데이터의집합

-describing the structure and constrant of database

데이터베이스구조와 제약사항이 묘사

#외부(external) 스키마
-공용의 으미보다는 어느 개인이나 특정 응용에 한정된 논리적 데이터 구조

-데이터베이스의 개별 사용자나 응용 프로그래머가 접근하는 데이터베이스를 정의

-사용자의 관점을 기술

#개념(Conceptual)스키마
-the overall logical structure

전체적으로 통합된 논리적 데이ㅓ 구조로서 접근권한,제약조건,보안 정책,무결성 규칙을 명세

-단순히 스키마라고도 하며 조직이나 기관 전체에서 정의

-모든 응용 시스템과 사용자가 필요로 하는 데이터를 통합한 조직 전체의 데이터베이스로 하나만 존재

only one it can exist per database

-범 기관적 입장에서 본 데이터베이스를 정의

#내부(Internal)스키마
-데이터베이스 시스템 구조에서 데이터가 실제로 저장되는 것과 관계

-물리적 저장장치의 입장에서 본 데이터베이스 구조

-실제로 데이터베이스에 저장될 레코드의 형식을 저장하고저장 데이터 항목의 표현방법, 내부 레코드의 물리적 순서등을 나타냄

-it defines how the data are physically arrranged on a storage device

데이터가 기억장치에 배치되는방법을 정의

-as seen by a system programmer or system designer

시스템 프로그래머나 시스템 디자이너 관점의 스키마

#데이터 정의 언어(DDL)
-데이터베이스,테이블,인덱스를 생성 및 삭제

-데이터베이스의 논리적 데이터 구조와 물리적 데이터 구조를 정의하거나 그 정의를 수정할 목적으로 사용

-번역한 결과가 데이터 사전이라는 특별한 파일에 여러 개의 테이블로서 저장된다.

-스키마,도메인,테이블,뷰,인덱스를 정의하고 변경하며 삭제

-SQL 유형 3가지: CREATE(정의),ALTER(변경),DROP(삭제)

#데이터 조작 언어(DML)
-데이터 처리를 위해 응용 프로그램과 DBMS 사이의 인터페이스 제공의 역할을 한다.

-SQL 유형 4가지: Select(레코드,자료,즉 튜플 검색),
                 Insert(튜플 삽입),
		 Update(튜플 갱신),
		 Delete(튜플 삭제)
		 (DELETE/=DROP)

#데이터 제어 언어(DCL)
-데이터의 보안,무결성,회복과 복구 및 병행 제어

-데이터베이스를 공용하기 위한 데이터 제어을 정의하고 기술

-제어어의 종류: SQL명령어로 수행된 결과를 실제 물리적 디스크로 저장
		ROLLBAK:비정상적으로 종료되었을때 복구
		GRANT:권한을 부여
		REVOKE:권한을 취소
