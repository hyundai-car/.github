# MyCarFor.me

 ![MyCarForMe](https://github.com/user-attachments/assets/8aa2938f-e22f-48aa-aaf3-59b44ce16b26)

## 1. 프로젝트 개요
[🍿 시연영상](https://www.youtube.com/watch?v=6WqxpxY3zD0)
> `MyCarForMe`는  처음부터 끝까지 원스톱으로 진행되는 중고차 거래 플랫폼으로,
 맞춤형 비교 분석과 실시간 배송 추적까지 제공합니다. 
 
 > 차량 검색부터 구매, 배송까지 최적화된 중고차 구매 경험을 실현할 수 있습니다.


### ⏳ 프로젝트 수행기간
2025.01.07 ~ 2025.01.21
![schedule](https://github.com/user-attachments/assets/2f927382-f940-4755-870e-0230c2be3d7f)

### 💻 기술스택
<table> <thead> <tr> <th>분류</th> <th>기술 스택</th> </tr> </thead> <tbody> <tr> <td> <p>Frontend</p> </td> <td> <img src="https://img.shields.io/badge/React 18.3.1-61DAFB?logo=react&logoColor=ffffff"> <img src="https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=ffffff"> <img src="https://img.shields.io/badge/Vite-646CFF?logo=vite&logoColor=ffffff"> <img src="https://img.shields.io/badge/pnpm-F69220?logo=pnpm&logoColor=ffffff"> <img src="https://img.shields.io/badge/Nginx-009639?logo=nginx&logoColor=ffffff"> <img src="https://img.shields.io/badge/Zustand-000000?logo=zustand&logoColor=ffffff"> <img src="https://img.shields.io/badge/React Query-FF4154?logo=react-query&logoColor=ffffff"> <img src="https://img.shields.io/badge/Chart.js-FF6384?logo=chart.js&logoColor=ffffff"> <img src="https://img.shields.io/badge/Android Studio-3DDC84?logo=android-studio&logoColor=ffffff"> <img src="https://img.shields.io/badge/Kotlin-7F52FF?logo=kotlin&logoColor=ffffff"> </td> </tr> <tr> <td> <p>Backend</p> </td> <td> <img src="https://img.shields.io/badge/Spring Boot 3.4.1-6DB33F?logo=springboot&logoColor=ffffff"> <img src="https://img.shields.io/badge/Spring Data JPA-6DB33F?logo=spring&logoColor=ffffff"> <img src="https://img.shields.io/badge/Spring Security-6DB33F?logo=springsecurity&logoColor=ffffff"> <img src="https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=ffffff"> <img src="https://img.shields.io/badge/Keycloak-33A6E8?logo=keycloak&logoColor=ffffff"> <img src="https://img.shields.io/badge/Docker-2496ED?&logo=docker&logoColor=white"> <img src="https://img.shields.io/badge/Thymeleaf-005F0F?logo=thymeleaf&logoColor=ffffff"> <img src="https://img.shields.io/badge/Swagger-85EA2D?logo=swagger&logoColor=ffffff"> <img src="https://img.shields.io/badge/FCM-FFCA28?logo=firebase&logoColor=ffffff"> <img src="https://img.shields.io/badge/Cool SMS-000000?"> </td> </tr> <tr> <td> <p>Infra</p> </td> <td> <img src="https://img.shields.io/badge/AWS EC2-FF9900?logo=amazonec2&logoColor=ffffff"> <img src="https://img.shields.io/badge/AWS RDS-527FFF?logo=amazonrds&logoColor=ffffff"> <img src="https://img.shields.io/badge/GitHub Actions-2088FF?logo=github-actions&logoColor=ffffff"> </td> </tr> </tbody> </table>

### 🏗️ 시스템 아키텍처
<img width="1280" alt="Image" src="https://github.com/user-attachments/assets/cd8e6f10-7da1-4748-a9de-163e87d17394" />

</details>

## 2. 주요 기능
![feature](https://github.com/user-attachments/assets/826592b0-b11b-4b60-9081-a3f5745834ee)


## 3. 수행 경과

### 💍 시퀀스 다이어그램
<details> <summary>  보기 </summary>
 
![payment](https://github.com/user-attachments/assets/88312975-c60c-4764-9139-965e6b8f0cdf)

![delivery](https://github.com/user-attachments/assets/f8c0e4fa-a563-481f-ae73-4e95aa47c811)

</details>
 
# Frontend 🍰

<details>
 
### ☑️ 기능 분할 설계(FSD)를 이용한 FE 아키텍처 구성 💻
### ☑️ FSD Debug 도구 도입 📂
### 중앙화된 에러 관리 전략 ⚠️
  - 라우팅 과정의 모든 에러를 상위 ErrorBoundary로 전파해 일관전 에러 처리 흐름 보장
### 중앙화된 경로 관리 시스템  📍
  - 경로 관리 시스템 Single Source of Truth 구현, pathKeys를 활용해 모든 경로를 중앙에서 관리
  - 모듈화를 통해 각 라우트를 독립된 파일로 관리  
### HOC 패턴을 활용한 코드 최적화 ✨
  - 재사용 가능한 Suspense 로직 구현 (WithSuspense)
  - Code Splitting을 위한 일관된 패턴 제공
  - 컴포넌트 레벨의 로딩 상태 관리
### 타입 시스템 강화 🔧
  - Zod를 활용한 런타임 유효성 검증, TypeScript의 타입 안정성 확보

## 트러블슈팅
### FSD 구조에서 계층 간 의존성 역전 이슈 발생 🔄
- 해결 : Slot 패턴을 통한 해결

</details>

# Backend ☕️

<details>
 
### ☑️ 중고차 데이터
1. AI 학습을 위한 학습용 데이터 수집(크롤링)과 전처리
2. 중고차 시세 예측 AI 모델 개발
3. 운영용 데이터 후처리 작업과 자체 가치 평가 기준 추가

### ☑️ Keycloak 인증서버 구현
![keycloak](https://github.com/user-attachments/assets/e753349b-524d-4b57-9f65-911a7a0af7c5)

### ☑️ 사용자의 선호도와 선택 조건에 기반한 차량 추천 시스템

</details>

 
## 🖐️ 팀원 소개

|                                                  정세진                                                   |                                                  곽혜정                                                   |                                                  윤서진                                                   |                                                  여진홍                                                   |                                                  정한얼                                                   |
| :-------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------: |
| <img src="https://github.com/user-attachments/assets/08ef3733-b926-4d56-bf0e-e0dfc49375a9" width="120" /> | <img src="https://github.com/user-attachments/assets/309d6327-b6c7-43a8-b916-cf7000a81457" width="120" /> | <img src="https://github.com/user-attachments/assets/16d6ea0f-2332-4ad1-9293-69efa2806325" width="120" /> | <img src="https://github.com/user-attachments/assets/26581220-4689-4237-b862-83797f80f0e1" width="120" /> | <img src="https://github.com/user-attachments/assets/5b129423-83d7-47ed-aa92-e3c6813e9424" width="120" /> |
|                                                  **FE/Android**                                                   |                                                  **FE/Design**                                                   |                                               **FE/Infra**                                                |                                                  **BE**                                                   |                                            **BE/Infra/AI**                                            |
|                                  [@jsj7878](https://github.com/jsj7878)                                   |                                 [@softourr](https://github.com/softourr)                                  |                                    [@jini9](https://github.com/jinii9)                                     |                                  [@zlnongi](https://github.com/zlnongi)                                   |                                   [@Haneol](https://github.com/Haneol)                                    |
