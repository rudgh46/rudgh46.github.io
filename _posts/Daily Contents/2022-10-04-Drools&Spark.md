---
title: "[Daily Contents] Drools & Spark"
categories:
  - Daily Contents
tags:
  - Daily Contents
  # -
toc: true
toc_sticky: true
toc_label: "Drools & Spark"
toc_icon: "bookmark"
---

<br>

## 빅데이터 프로젝트의 간단한 개요

1. 빅데이터 소스 // 데이터 소스(내부 데이터, 외부 데이터)
2. 빅데이터 수집 // 수집, 통합, 전처리(DB Connector, 검색 API)
   - 정형, 비정형 데이터 수집
   - 데이터 취합 후 저장
3. 빅데이터 구축 // 저장, 관리(MySQL)
   - 데이터 분산 저장
   - 필요 시 준 구조화된 데이터 저장
4. 빅데이터 분석 // 분석(PRO SINDI)
   - 초고속 병렬 처리
   - 데이터 가공, 추출
   - 데이터 분석 전처리
5. 빅데이터 활용 // 표현(가시화)
   - 데이터 보안, 권한
   - 데이터 품질, 백업
   - 플랫폼 시스템 관리

```
(2, 3) >> Operation
(4, 5) >> Analytics
```

## Drools와 BRMS

**Drools = (매우 빠르게)참 또는 거짓을 평가**

- Jboss에서 개발한 BRMS(business rule management system : 비즈니스 규칙 관리 시스템)
- 비즈니스 규칙 구현을 **자동화**하도록 설계된 Apache license 2.0 **OpenSource** solution.
- 비즈니스 규칙 및 의사 결정, 논리 정의, 배포, 실행, 모니터링 및 관리하는 데 사용되는 소프트웨어 솔루션으로, 비즈니스 규칙은 회사 또는 업계가 운영하는 회사 정책 또는 법률 및 규정을 기반으로 하며, 비즈니스 규칙은 작업들의 정의에 따라 항상 **참 또는 거짓을 평가**
- **BRMS**를 통해 기업은 **IT 직원의 개입 없이**도 새로운 운영 조건을 빠르게 적용 가능
- BRMS는 IT 부서에서 이러한 시스템을 수동으로 재구성하지 않고도 데이터베이스와 같은 IT 시스템에 대한 변경을 자동화함으로서 새로운 비즈니스 규칙을 구현하는 데 걸리는 시간을 줄일 수 있다.
- BRMS는 기술 및 비즈니스 사용자가 비즈니스 규칙을 정의하고 관리할 수 있는 **개발 도구를 제공**, 사용자는 **코드를 작성하지 않고** 비즈니스 규칙을 개발하는 중에도 비즈니스 규칙을 검증할 수 있다.
- 단점은 비즈니스 규칙을 정의하려면 **회사, 산업 및 규정에 대한 많은 지식이 필요하기 때문에** BRMS를 구현하기가 어렵다는 것
- **BPMS** : 비즈니스 **프로세스**를 최적화하여 효율성과 생산성을 높이도록 하는 소프트웨어 솔루션

**BRMS** : 비즈니스 규칙을 정의, 실행 및 관리하기 위한 시스템
**BPMS** : 비즈니스 프로세스를 최적화하여 효율성과 생산성을 높이는 시스템

**Low Code** : 선 개발된 모듈과 적은량의 개발, GUI 등의 간단한 조작으로 조합하여 시스템을 만드는 개발 방법.
**RPA** : (반복적인 작업을 처리하는) "로봇을 이용한 프로세스의 자동화"로 비용과 인원을 줄이는 것

**No Code**

## Hadoop MapReduce

- Master worker >>(작업 부여, 매핑)>> Sub workers
- Recude : 매핑한 작업의 응답을 받아 최적화하는 과정 <br>
  **Based on - HDFS**

## Apache Spark

**RDD : Resilient Distributed Datasets**

|                 | Spark                                                       | Hadoop MapReduce                |
| --------------- | ----------------------------------------------------------- | ------------------------------- |
| speed           | 100x times than MapReduce                                   | Faster than traditional system  |
| Written in      | Scala                                                       | Java                            |
| Data Processing | Batch, real-time. iterative, interactive, graph             | Batch processing                |
| Ease of Use     | Compact & easier than Hadoop                                | Complex & lengthy               |
| Caching         | Caches the data in-memory & enhances the system performance | Doesn't support caching of data |

## Data Flow

## (사례) 쿠팡 데이터 플랫폼 변천사

## A Unified Data Infrastructure Architecture

## Drools의 미래?

## 참고

- 2017년 한국정보통신학회 발간, 한국정보통신학회 논문지 - 아파치 스파크 기반 검색엔진의 설계 및 구현 논문
- SK 인포섹 EQST 그룹 - 오픈 소스 소프트웨어 보안 가이드
- Youtube - 최신 데이터 인프라 이해하기
