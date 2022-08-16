---
title: "데이터베이스 언어(SQL)의 종류"
date: 2022-07-23T01:02:36+09:00
draft: false
---

## DDL

데이터베이스를 정의하는 언어이며, 데이터를 생성, 수정, 삭제하는 등의 데이터의 전체의 골격을 결정하는 역할을 하는 언어이다.

### DDL의 종류

- `CREATE` : 데이터베이스, 테이블등을 생성
- `ALTER` : 테이블을 수정
- `DROP` : 데이터베이스, 테이블등을 삭제
- `TRUNCATE` : 테이블을 초기화

## DML

데이터베이스에 등록된 레코드를 조회,수정,삭제하는 등의 역할을 하는 언어이다.

### DML의 종류

- `SELECT` : 데이터를 조회
- `INSERT` : 데이터를 삽입
- `UPDATE` : 데이터를 수정
- `DELETE` : 데이터를 삭제

## DCL

데이버테이스에 접근하거나 객체에 권한을 주는 등의 역할을 하는 언어이다.

### DCL의 종류

- `GRANT` : 데이터베이스 사용자에게 사용 권한을 부여
- `REVOKE` : 데이터베이스 사용자의 사용 권한을 회수
- `COMMIT` : 데이터베이스 조작 작업을 영구적으로 반영하여 완료
- `ROLLBACK` : 데이터베이스 조작 작업이 비정상적으로 종료되었을 때 원래의 상태로 복구

---

DDL: Data Definition Language, 데이터 정의어  
DML: Data Manipulation Language, 데이터 조작어  
DCL: Data Control Language, 데이터 제어어
