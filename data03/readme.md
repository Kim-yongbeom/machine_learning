# mysql

### 트랜잭션(Transaction)은 데이터베이스의 완전성을 보장하기 위한 것입니다. 상태를 변화시키기 해서 수행하는 하나의 작업의 단위를 뜻합니다.

### root에서 유저설정

  - 유저 생성
    - create user 원하는이름@localhost identified by '원하는비밀번호!';
    - 만든 아이디로 접속하려면 mysql -u 원하는이름 -p

  - 보안설정
    - grant all privileges on  *.* to '설정한이름'@'localhost';

### 데이터 베이스 만들기
- create database 원하는이름

### 데이터 베이스 사용하기
- use bigdata;

### 테이블 만들기
- create table 원하는이름 ( id varchar(100), pw varchar(100), name varchar(100), tel varchar(100));
- create table 원하는이름 ( id int primary key auto_increment, pw varchar(100), name varchar(100), tel varchar(100));

### 테이블 row생성
- insert into 테이블명 values ('200','200','200','200');

### 테이블 row삭제
- DELETE FROM plan WHERE 컬럼명=100;

### 테이블 row확인
- select * from 테이블명;

### 자동 커밋확인하기
- select @@autocommit;

### 수동 커밋
- set @@autocommit = 0; 
- commit;

### 행 추가 취소 (마지막 커밋 이후)
- rollback;

### DBeaver로 데이터베이스 백업
<img width="472" alt="스크린샷 2021-12-20 오전 11 55 30" src="https://user-images.githubusercontent.com/89058117/146705325-800b8c13-3ba9-4eb2-981c-ac055996b03d.png">
- 백업할 데이터베이스 dump
- 받을 데이터베이스 생성 후 restore 누르면 파일 선택할 폴더 열림 그 폴더에서 sql 파일 선택

### DBeaver에서 데이터베이스에 csv 파일 넣기
<img width="371" alt="스크린샷 2021-12-20 오후 12 18 48" src="https://user-images.githubusercontent.com/89058117/146706916-2abfea58-9d32-424e-bc7b-149ae5e7c5df.png">

### DBeaver에서 외래키 설정
<img width="707" alt="스크린샷 2021-12-20 오후 5 35 00" src="https://user-images.githubusercontent.com/89058117/146737210-d3f19847-bf52-4b67-b6c1-8d1def33a85c.png">


### 데이터프레임 다루기
- 1. 데이터를 분석하기전 행렬구조의 데이터를 넣는 구조는?  '데이터프레임'
- 2. 1번의 데이터 구조를 사용하기 위한 라이브러리는?    'pandas'
- 3. 판단하기 적합한 선을 찾거나, 랜덤한 샘플 데이터를 만들기 위한 라이브러리는?    'seaborn'
- 4. 데이터 분석과정 plot으로 확인하거나, 최종 분석 결과를 표현하기 위한 plot을 사용한다. 이때 필요한 라이브러리는?    'matplotlib'
- 5. 데이터 프레임에서 행과 열을 삭제하는 함수는?    'drop()'
- 6. 두 데이터프레임을 조인할 때 행과 열을 합하는 함수는?   'concat()'
  - 컬럼이 똑같을때만 가능(ignore_index=True를 넣어줘야 인덱스가 올바르게 들어감), (join='inner')넣어주면 공통된 컬럼만 출력
- 7. 데이터 프레임에서 두 항목의 상관 관계를 알기위한 함수는?     'corrcoef()'
  - 이 상관관계를 나타내는 숫자를 무엇이라고 하는가?     '상관계수'
  - 이 상관관계를 나타내는 숫자의 범위는?    '0 ~ 1'
- 8. 7번의 결과가 0.78이 나왔다. 어떻게 판단하는가?    '강한 상관관계'
- 9. 데이터의 흩어져 있는 정도를 그릴 수 있는 plot은? 한글/영문    '?'
- 10. 흩어져 있는 정도를 보고, plot위에 판단의 적정 기준선을 그려 넣고 싶다. 기준선을 넣기 위한 방법을 순서대로 함수를 이용하여 설명하시오.     '?'














