<p align="center">
    <img width="200px;" src="https://raw.githubusercontent.com/woowacourse/atdd-subway-admin-frontend/master/images/main_logo.png"/>
</p>
<p align="center">
  <img alt="npm" src="https://img.shields.io/badge/npm-%3E%3D%205.5.0-blue">
  <img alt="node" src="https://img.shields.io/badge/node-%3E%3D%209.3.0-blue">
  <a href="https://edu.nextstep.camp/c/R89PYi5H" alt="nextstep atdd">
    <img alt="Website" src="https://img.shields.io/website?url=https%3A%2F%2Fedu.nextstep.camp%2Fc%2FR89PYi5H">
  </a>
  <img alt="GitHub" src="https://img.shields.io/github/license/next-step/atdd-subway-service">
</p>

<br>

# 인프라공방 샘플 서비스 - 지하철 노선도

<br>

## 🚀 Getting Started

### Install

#### npm 설치

```
cd frontend
npm install
```

> `frontend` 디렉토리에서 수행해야 합니다.

### Usage

#### webpack server 구동

```
npm run dev
```

#### application 구동

```
./gradlew clean build
```

<br>

## 미션

* 미션 진행 후에 아래 질문의 답을 작성하여 PR을 보내주세요.

### 1단계 - 화면 응답 개선하기

1. 성능 개선 결과를 공유해주세요 (Smoke, Load, Stress 테스트 결과)

2. 어떤 부분을 개선해보셨나요? 과정을 설명해주세요

---

### 2단계 - 조회 성능 개선하기

1. 인덱스 적용해보기 실습을 진행해본 과정을 공유해주세요
    1. 쿼리최적화
        1. [data-tuning.sql] (https://github.com/All-ForOne/infra-subway-performance/blob/7aa4b62c944399c5981668b976885e2b340e853d/src/main/resources/data-tuning.sql) 에 작성한 쿼리로 실행시 수행시간 0.313 초
        2. 사원출입기록 테이블에 (사원번호, 지역, 입출입구분) 인덱스 추가 후 수행시간 0.016 초
    2. 인덱스설계  
       [index.sql] (https://github.com/All-ForOne/infra-subway-performance/blob/7aa4b62c944399c5981668b976885e2b340e853d/src/main/resources/index.sql)

2. 페이징 쿼리를 적용한 API endpoint를 알려주세요  
https://all-forone.p-e.kr/stations?offset=0&size=10

