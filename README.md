
![image](https://github.com/user-attachments/assets/32b69b7f-c8f1-4a49-9bd6-73cb6723698d)

# **Together**
## 프로젝트 소개
- "특정 여행지" 에서 "특정 일정"에 나와 동행할 수 있는 "적절한 누군가" 를 찾고싶다.
- 지역별 여행지 / 일정을 정리해서 동행자를 찾을 수 있는 어플리케이션
- 전세계 유저를 대상으로 하며, MVP 를 먼저 출시하여 실제 수요를 확인하고자 한다.

## Contributors

- 팀장 : 박성준
- 1~2일차 팀원 : 임건우, 박소은, 김택준
- 3~4일차 팀원 : 이재윤, 양상원

## 협업 도구
- Google Sheets : 요구사항 명세서 / 기능 명세서
- Figma : UI 설계
    - FigJam : UI 초안 작성
- ERD 작성 : ERD Cloud
- API 명세 작성 : Notion 

## 산출물
### 요구사항 명세서
[Google Sheets - 요구사항 명세서](https://docs.google.com/spreadsheets/d/1JWTPQIfjt_Tpc1RSI6gckm-ssMxSHy9X5MA9IFc1_II/edit?usp=sharing)

### ERD
[ERD Cloud](https://www.erdcloud.com/d/Ey749xad75dJxgE6K)

![image](https://github.com/user-attachments/assets/0f4957a4-3cb3-4adb-881a-cd83b794f21d)

### API 명세서

[Notion - API 명세](https://www.notion.so/API-d4a4d7d4958f4ca7befab0cbb738ba57?pvs=4)

### 화면 구성

[Figma](https://www.figma.com/design/MgS77UV2lBz9W6SaGh3lNx/Mobile-App-Design?node-id=0-1&t=D2CwxtwH6Ynia0A9-1)

#### 프로필
![image](https://github.com/user-attachments/assets/732dd22d-4872-41ec-8436-f9a8aaab67ff) | ![image](https://github.com/user-attachments/assets/732dd22d-4872-41ec-8436-f9a8aaab67ff) | ![image](https://github.com/user-attachments/assets/efec482c-ef55-4a10-81a3-81d7fb961331)
---|---|---|


#### 여행 일정

![image](https://github.com/user-attachments/assets/abf93eca-5428-40fe-ac83-45be4f118059) | ![image](https://github.com/user-attachments/assets/ac27e3df-ce8b-4d26-a14b-d98f7e89495f) | ![image](https://github.com/user-attachments/assets/b1f43bf3-0587-41d0-b7f0-82d7f630d291) | ![image](https://github.com/user-attachments/assets/f43d4da4-787f-4a32-9702-8ebe2ba93cec)
---|---|---|---|

#### 채팅

![image](https://github.com/user-attachments/assets/a0a3effd-b6ee-4801-b8f7-ece84a48f40e) | ![image](https://github.com/user-attachments/assets/551cca60-5fcc-4378-8dac-8c1742950e46)
---|---|

## 시스템 아키텍처

![image](https://github.com/user-attachments/assets/aef656ac-4771-419a-bccd-527c27cd221e)


## 기술 스택

- 아직 수요가 미지수인 어플리케이션 출시를 가정하였습니다.
    
    ### 서버
    
    #### 언어 및 프레임 워크
    
    - Java 17, Spring Boot 3.3.x
    
    #### DB
    
    - MySQL 8.x
    
    ### 클라이언트
    
    - React Native
        - 푸시 알림, 대상 사용자를 고려할 때 모바일 앱으로 배포가 필요하였다.
        - Native 앱의 경우 iOS / Android 개별 개발이 필요한데, 현재 빠르게 서비스를 배포한다는 목적에 부합하지 않았다.
        - 일반적으로 웹 개발자의 경우 js 에 익숙하며 함께 개발에 빠르게 참여할 수 있다는 점을 이유로 선정하였다.
    
    ### 인프라
    
    - AWS Cloud
        - ECS (Backend API Server) - Fargate
            - ECR for container registry
        - RDS for MySQL DB Instance
            - 안정적인 DB 운영
        - S3
            - image 업로드 및 저장을 위함
        - 모니터링에 대한 기술 선택이 필요하지만 현재 해당 사항까지 고려하지 못하였다.
    - Firebase Cloud Messaging
        - 모바일 푸시 알림
    
    ### 사용하는 외부 API
    
    - Google / Kakao / Apple OAuth
    - Google 지도 API
        - 국내보다 글로벌 서비스를 타깃으로 잡고 있어 Google API 활용이 가장 적합함.

## 발표자료
[Google slide](https://docs.google.com/presentation/d/1TdRTxUEhZu2otAOfha70xBANcTtQy-iWhpby3w7MhZw/edit?usp=sharing)
