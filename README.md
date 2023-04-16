# effective-mysql

## 실무적인 SQL 튜닝 절차

가시적:
- 테이블 데이터 건수
- SELECT절 컬럼 분석
- 조건절 컬럼 분석
- 그루핑/정렬 컬럼

비가시적:
- 실행계획
- 인덱스 현황
- 데이터 변경 추이
- 업무적 특징

## SQL 힌트

STRAIGHT_JOIN - FROM 절에 작성된 테이블 순으로 조인 유도
USE INDEX - 특정 인덱스를 사용하도록 유도
FORCE INDEX - 특정 인덱스를 사용하도록 강제
IGNORE INDEX - 특정 인덱스를 사용하지 못하게 유도

## 절차(How)가 아닌 대상(What)을 기술하는 언어

SQL는 간단한 언어가 아니다.

HOW를 의식하는 것이 SQL 튜닝의 첫 걸음

## 통계 정보 갱신

ANALYZE TABLE [스키마 이름].[테이블 이름]

## I/O 
### 논리적 I/O vs 물리적 I/O
### 시퀀셜 액세스 vs 랜덤 액세스
### Single Block I/O vs Multiblock I/O

## [DBeaver] MySQL 연결 시 "Public Key Retrieval is not allowed" 해결하기

https://velog.io/@dailylifecoding/DBeaver-MySQL-connecting-error-Public-Key-Retrieval-is-not-allowed-solved


## [MySQL] Binary Log 관련 명령

https://myinfrabox.tistory.com/149


## ib_logfile(Redo log),

https://myinfrabox.tistory.com/259

## performance schema

https://myinfrabox.tistory.com/194
