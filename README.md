# Together
여행지에서 동행을 구하고 싶을 때, 새로운 사람을 만나고 싶을 때 **Together**!

## 기획 의도
- "특정 여행지" 에서 "특정 일정"에 나와 동행할 수 있는 "적절한 누군가" 를 찾고싶다.
- 지역별 여행지 / 일정을 정리해서 동행자를 찾을 수 있는 어플리케이션

## 요구사항 명세서 / 기능 명세서
[Google Sheet - 요구사항 명세서](https://docs.google.com/spreadsheets/d/1JWTPQIfjt_Tpc1RSI6gckm-ssMxSHy9X5MA9IFc1_II/edit?gid=1070321515#gid=1070321515) 

## ERD
[ERD Cloud](https://www.erdcloud.com/d/Ey749xad75dJxgE6K)

## UI 초안
[FigJam](https://www.figma.com/board/0EHVPpTtKET5LeNlzMYwF3/Together?node-id=0-1&t=syKinN0ja1cVFWEZ-0)

## 기술 스택
(아직 정확하게 결정된 상태 아닙니다.)
### Backend
- Java 17 + Spring Boot 3.x
  - Spring Data JPA + Spring Security
- MySQL 8

### Frontend
- Mobile 위주로 구성할 계획을 세우고 있습니다.
- App -> Flutter / React native / Next.js

### Infra
- AWS cloud 이용
  - API Server : EC2
  - DB : RDS
  - Image Bucket : S3
