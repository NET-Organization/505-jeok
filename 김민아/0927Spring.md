## 📝 오늘 공부한 내용
> 예술적인 소프트웨어 프로젝트 트러블 슈팅

## 😲 오늘 깨달은 내용
자꾸 객체 조회를 수행할 때 에러가 나길래 봤더니 userId와 날짜로 조회하는 메서드에 오류가 있었다. 알 수 없는 이유로 똑같은 유저 아이디와 날짜로 여러개의 객체가 생성돼서 SQL쿼리 수행 결과가 unique하지 않아서 에러가 난 것 같다.
그래서 DB에서 SQL 구문으로 직접 삭제를 하려고 했더니 외래키 제약 조건 때문에 일대다 매핑돼있던 counselingLog와 calendars 테이블에 있는 레코드를 삭제할 수 없어서 코드에 cascade 조건을 추가했다. 

## 🥲 오늘 이해못했거나 궁금한 내용
AWS에서 IAM에 EC2 권한을 줬는데 대체 왜 내가 EC2를 관리할 수 없는지 너무 짜증난다;; 맨날 수진이한테 ec2 재부팅 해달라고 싹싹 빌어야돼서 미안해 죽겠다 ㅠㅠㅠㅠ

## 📁 참고한 자료 및 사진 첨부
- 챗지피티
