# 🧞‍♂️ 캐톡 (Character Talk) 🎅🏻

## 💻 `프로젝트 소개 & 개발 동기`

<br/>

## 🧑‍🤝‍🧑 `멤버구성 & 담당한 역할`

 - 팀장: 이득규
   - TTS 음성 트레이닝
   - 인기 캐릭터 조회수
   - 김전일 프롬프트 작성
     
 - 형상관리자: 홍주연
   - 1:1 채팅 기능 구현
   - 단체 채팅 기능 구현
   - 감정 분석된 이미지 라우팅
   - 채팅 내역 기억 및 페이징 처리
   - FAST API 시작 시 각 캐릭터 정보 retriever로 서버에 로드 및 벡터 스토어 저장
   - 스폰지밥/버즈 프롬프트 작성

 - 형상관리자: 지동현
   - 구글/카카오 로그인
   - 단체방 생성
   - 백엔드에서 채팅방 정보를 요청하여 화면단에 반영
   - 네비게이션 바, 채팅방 디자인
   - 리바이 프롬프트 작성
  
 - 리뷰어: 배하은
   - 메인페이지, 채팅방, 밸런스 게임 선택지 디자인
   - 밸런스 게임 프롬프트 작성
   - 에스카노르 낮/밤 프롬프트 작성

 - 리뷰어: 박효찬
   - 네비게이션 바 디자인 및 구현
   - 최근 채팅한 방 정보 네비게이션 바에 불러오기
   - 플랑크톤 프롬프트 작성

<br/>

## ⚙️ `개발 환경`
![skills](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![skills](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=JavaScript&logoColor=white)
![skills](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![skills](https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![skills](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![skills](https://img.shields.io/badge/axios-671ddf?&style=for-the-badge&logo=axios&logoColor=white)
![skills](https://img.shields.io/badge/Redux-593D88?style=for-the-badge&logo=redux&logoColor=white)

![skills](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![skills](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)
![skills](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)
![skills](https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=Spring-Security&logoColor=white)
![skills](https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=Hibernate&logoColor=white)
![skills](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![skills](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![skills](https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=Swagger&logoColor=white)

![skills](https://img.shields.io/badge/IntelliJ_IDEA-000000.svg?style=for-the-badge&logo=intellij-idea&logoColor=white)
![skills](https://img.shields.io/badge/VSCode-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white)
![skills](https://img.shields.io/badge/Sourcetree-0052CC?style=for-the-badge&logo=Sourcetree&logoColor=white)
![skills](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=Postman&logoColor=white)
![skills](https://img.shields.io/badge/IntelliJ_IDEA-000000.svg?style=for-the-badge&logo=intellij-idea&logoColor=white)
![skills](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)
![skills](https://img.shields.io/badge/Canva-%2300C4CC.svg?&style=for-the-badge&logo=Canva&logoColor=white)
![skills](https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white)

<br/>
<br/><h2>📂 패키지구조</h2>

<details>
  <summary><b>프론트엔드 패키지 구조</b></summary>
  <div markdown="1">

```
C:.
|   .env
|   .gitignore
|   package-lock.json
|   package.json
|   README.md
|   tree.txt
|   
+---public
|   |   c-talk.ico
|   |   c-talk.png
|   |   index.html
|   |   manifest.json
|   |   robots.txt
|   |   
|   \---images
|           google_logo.png
|           icon-login.png
|           icon-login2.png
|           kakao_logo.png
|           캐릭터1.png
|           캐릭터2.png
|           캐릭터3.png
|           
\---src
    |   App.js
    |   index.js
    |   ProtectedRoute.js
    |   Store.js
    |   TestPage.js
    |   
    +---apis
    |       Apis.js
    |       ChatAPICalls.js
    |       ImageAPICalls.js
    |       UserAPICalls.js
    |       
    +---components
    |   |   GroupChatFormModal.js
    |   |   LoginModal.js
    |   |   ProfileModal.js
    |   |   
    |   \---commons
    |           Navbar.js
    |           
    +---css
    |       balanceChat.css
    |       balanceGame.css
    |       chat.css
    |       GroupChatFormModal.css
    |       LoginModal.css
    |       Navbar.css
    |       ProfileModal.css
    |       selectCharacterList.css
    |       UserMain.css
    |       
    +---images
    |       icon.png
    |       mypage.png
    |       
    +---layouts
    |       Layout.js
    |       
    +---modules
    |       ChatModule.js
    |       ImageModule.js
    |       index.js
    |       UserModule.js
    |       
    \---pages
        |   UserMain.js
        |   
        +---balanceGame
        |   |   balanceChat.js
        |   |   balanceGame.js
        |   |   
        |   \---images
        |           Refresh.png
        |           Sms.png
        |           김전일.jpg
        |           리바이.webp
        |           버즈.jpg
        |           상황1.png
        |           스폰지밥.jpg
        |           에스카노르.jpg
        |           플랑크톤.jpg
        |           
        +---chat
        |   |   BalanceMessage.js
        |   |   ChatRoom.js
        |   |   Message.js
        |   |   
        |   \---images
        |           Button Play.png
        |           down.png
        |           list_icon.png
        |           loading1.gif
        |           loading2.gif
        |           loading3.gif
        |           loading4.gif
        |           loading5.gif
        |           loading6.gif
        |           
        +---selectCharacterList
        |   |   selectCharacterList.js
        |   |   
        |   \---images
        |           icon.png
        |           
        \---user
                Login.js
```
    
  </div>
</details>


<details>
  <summary><b>백엔드 패키지 구조</b></summary>
  <div markdown="1">

```
C:.
|   .gitattributes
|   .gitignore
|   build.gradle
|   gradlew
|   gradlew.bat
|   HELP.md
|   settings.gradle
|   tree.txt
|   
+---.gradle
|   |   file-system.probe
|   |   
|   +---8.10.2
|   |   |   gc.properties
|   |   |   
|   |   +---checksums
|   |   |       checksums.lock
|   |   |       md5-checksums.bin
|   |   |       sha1-checksums.bin
|   |   |       
|   |   +---dependencies-accessors
|   |   |       gc.properties
|   |   |       
|   |   +---executionHistory
|   |   |       executionHistory.bin
|   |   |       executionHistory.lock
|   |   |       
|   |   +---expanded
|   |   +---fileChanges
|   |   |       last-build.bin
|   |   |       
|   |   +---fileHashes
|   |   |       fileHashes.bin
|   |   |       fileHashes.lock
|   |   |       resourceHashesCache.bin
|   |   |       
|   |   \---vcsMetadata
|   +---buildOutputCleanup
|   |       buildOutputCleanup.lock
|   |       cache.properties
|   |       outputFiles.bin
|   |       
|   \---vcs-1
|           gc.properties
|           
+---.idea
|   |   .gitignore
|   |   compiler.xml
|   |   dataSources.local.xml
|   |   dataSources.xml
|   |   gradle.xml
|   |   jarRepositories.xml
|   |   misc.xml
|   |   modules.xml
|   |   sqldialects.xml
|   |   vcs.xml
|   |   workspace.xml
|   |   
|   +---dataSources
|   |   |   270ef987-d471-4581-a575-0672e3593532.xml
|   |   |   
|   |   \---270ef987-d471-4581-a575-0672e3593532
|   |       \---storage_v2
|   |           \---_src_
|   |               \---schema
|   |                       dlp_db.NePKsA.meta
|   |                       
|   \---modules
|           DLP_back.main.iml
|           
+---gradle
|   \---wrapper
|           gradle-wrapper.jar
|           gradle-wrapper.properties
|           
\---src
    +---main
    |   +---java
    |   |   \---com
    |   |       \---dlp
    |   |           \---back
    |   |               |   characterTalk.java
    |   |               |   
    |   |               +---auth
    |   |               |   |   AuthController.java
    |   |               |   |   RestTemplateConfig.java
    |   |               |   |   
    |   |               |   +---filter
    |   |               |   |       HeaderFilter.java
    |   |               |   |       JwtAuthorizationFilter.java
    |   |               |   |       
    |   |               |   +---handler
    |   |               |   |       JwtTokenProvider.java
    |   |               |   |       
    |   |               |   \---service
    |   |               |           CustomUserDetails.java
    |   |               |           CustomUserDetailsService.java
    |   |               |           
    |   |               +---character
    |   |               |   +---controller
    |   |               |   |       CharacterController.java
    |   |               |   |       
    |   |               |   +---domain
    |   |               |   |   +---dto
    |   |               |   |   |       CharacterDTO.java
    |   |               |   |   |       
    |   |               |   |   \---entity
    |   |               |   |           Character.java
    |   |               |   |           
    |   |               |   +---repository
    |   |               |   |       CharacterRepository.java
    |   |               |   |       
    |   |               |   \---service
    |   |               |           CharacterService.java
    |   |               |           
    |   |               +---chatMessage
    |   |               |   +---controller
    |   |               |   |       ChatMessageController.java
    |   |               |   |       
    |   |               |   +---domain
    |   |               |   |   +---dto
    |   |               |   |   |       CharacterMatchRequest.java
    |   |               |   |   |       CharacterMatchRequestFastAPI.java
    |   |               |   |   |       CharacterMatchResponseFastAPI.java
    |   |               |   |   |       ChatMessageDTO.java
    |   |               |   |   |       ChatRequest.java
    |   |               |   |   |       ChatRequestFastAPI.java
    |   |               |   |   |       ChatResponseFastAPI.java
    |   |               |   |   |       DeleteUserMessageRequest.java
    |   |               |   |   |       MsgImgRequest.java
    |   |               |   |   |       
    |   |               |   |   \---entity
    |   |               |   |           ChatMessage.java
    |   |               |   |           
    |   |               |   +---repository
    |   |               |   |       ChatMessageRepository.java
    |   |               |   |       
    |   |               |   \---service
    |   |               |           ChatMessageService.java
    |   |               |           
    |   |               +---chatRoom
    |   |               |   +---controller
    |   |               |   |       ChatRoomController.java
    |   |               |   |       
    |   |               |   +---domain
    |   |               |   |   +---dto
    |   |               |   |   |       ChatRoomDTO.java
    |   |               |   |   |       ChatRoomInfo.java
    |   |               |   |   |       ChatRoomResponse.java
    |   |               |   |   |       ChatRoomResponse2.java
    |   |               |   |   |       CreateChatRoomDTO.java
    |   |               |   |   |       GroupChatRoomInfo.java
    |   |               |   |   |       UpdateChatRoomDTO.java
    |   |               |   |   |       
    |   |               |   |   \---entity
    |   |               |   |           ChatRoom.java
    |   |               |   |           
    |   |               |   +---repository
    |   |               |   |       ChatRoomRepository.java
    |   |               |   |       
    |   |               |   \---service
    |   |               |           ChatRoomService.java
    |   |               |           
    |   |               +---common
    |   |               |       AuthConstants.java
    |   |               |       ResponseMessage.java
    |   |               |       
    |   |               +---config
    |   |               |       BeanConfiguration.java
    |   |               |       SwaggerConfig.java
    |   |               |       WebSecurityConfig.java
    |   |               |       
    |   |               +---images
    |   |               |   +---controller
    |   |               |   |       ImagesController.java
    |   |               |   |       
    |   |               |   +---domain
    |   |               |   |   +---dto
    |   |               |   |   |       ImagesDTO.java
    |   |               |   |   |       
    |   |               |   |   \---entity
    |   |               |   |           Images.java
    |   |               |   |           
    |   |               |   +---repository
    |   |               |   |       ImagesRepository.java
    |   |               |   |       
    |   |               |   \---service
    |   |               |           ImagesService.java
    |   |               |           S3Service.java
    |   |               |           
    |   |               +---member
    |   |               |   +---controller
    |   |               |   |       MemberController.java
    |   |               |   |       
    |   |               |   +---domain
    |   |               |   |   +---dto
    |   |               |   |   |       MemberDTO.java
    |   |               |   |   |       UpdateMemberDTO.java
    |   |               |   |   |       
    |   |               |   |   \---entity
    |   |               |   |           Member.java
    |   |               |   |           
    |   |               |   +---repository
    |   |               |   |       MemberRepository.java
    |   |               |   |       
    |   |               |   \---service
    |   |               |           MemberService.java
    |   |               |           
    |   |               \---participant
    |   |                   +---controller
    |   |                   |       ParticipantController.java
    |   |                   |       
    |   |                   +---domain
    |   |                   |   +---dto
    |   |                   |   |       ParticipantDTO.java
    |   |                   |   |       
    |   |                   |   \---entity
    |   |                   |           Participant.java
    |   |                   |           
    |   |                   +---repository
    |   |                   |       ParticipantRepository.java
    |   |                   |       
    |   |                   \---service
    |   |                           ParticipantService.java
    |   |                           
    |   \---resources
    |       |   application.yml
    |       |   Dummies.sql
    |       |   table_sessionId.sql
    |       |   
    |       +---static
    |       |   \---image
    |       |       +---characterProfile
    |       |       |       김전일.png
    |       |       |       리바이.png
    |       |       |       버즈.png
    |       |       |       스폰지밥.png
    |       |       |       에스카노르.png
    |       |       |       플랑크톤.png
    |       |       |       
    |       |       \---msgImg
    |       |           +---1
    |       |           |       1_1.jpg
    |       |           |       1_2.jpg
    |       |           |       1_3.jpg
    |       |           |       1_4.jpg
    |       |           |       1_5.jpg
    |       |           |       1_6.jpg
    |       |           |       1_7.jpg
    |       |           |       1_8.jpg
    |       |           |       2_1.jpg
    |       |           |       2_2.jpg
    |       |           |       2_3.jpg
    |       |           |       
    |       |           +---2
    |       |           |       1.jpg
    |       |           |       
    |       |           +---3
    |       |           |       1.jpg
    |       |           |       2_1.jpg
    |       |           |       2_2.jpg
    |       |           |       2_3.jpg
    |       |           |       2_4.jpg
    |       |           |       2_5.jpg
    |       |           |       2_6.jpg
    |       |           |       2_7.jpg
    |       |           |       2_8.jpg
    |       |           |       
    |       |           +---4
    |       |           |       1_1.jpg
    |       |           |       1_2.jpg
    |       |           |       1_3.jpg
    |       |           |       2_1.jpg
    |       |           |       2_2.jpg
    |       |           |       2_3.jpg
    |       |           |       2_4.jpg
    |       |           |       
    |       |           +---5
    |       |           |       1_1.jpg
    |       |           |       1_2.jpg
    |       |           |       1_3.jpg
    |       |           |       1_4.jpg
    |       |           |       1_5.jpg
    |       |           |       2_1.jpg
    |       |           |       2_2.jpg
    |       |           |       2_3.jpg
    |       |           |       
    |       |           \---6
    |       |                   1_1.jpg
    |       |                   1_2.jpg
    |       |                   1_3.jpg
    |       |                   1_4.jpg
    |       |                   1_5.jpg
    |       |                   1_6.jpg
    |       |                   1_7.jpg
    |       |                   2_1.jpg
    |       |                   2_2.jpg
    |       |                   2_3.jpg
    |       |                   2_4.jpg
    |       |                   
    |       \---templates
    \---test
        \---java
            \---com
                \---dlp
                    \---back
                            characterTalkTests.java
```
    
  </div>
</details>

<details>
  <summary><b>Fast API 패키지 구조</b></summary>
  <div markdown="1">

```
C:.
|   .env
|   .gitignore
|   chat_logic.py
|   main.py
|   models.py
|   tree.txt
|   TTS.py
|   
+---.vscode
|       settings.json
|       
\---data
        김전일.pdf
        리바이.pdf
        버즈.pdf
        스폰지밥.pdf
        에스카노르.pdf
        플랑크톤.pdf
```
    
  </div>
</details>


<br/>
<br/><h2>📌 주요 기능</h2>

<br/><h3>👾 회원가입 및 로그인 👾</h3>
- ~~~

<br/><h3>🧚‍♀️ 1:1 채팅 🧚‍♂️</h3>
- TODO: 각각 캐릭터마다 설명 & 음성 & 이미지 라우팅

<br/><h3>🧛‍♀️ 단체 채팅 🧛‍♂️</h3>
- TODO: who to send 모델 설명

<br/><h3>🕵️‍♂️ 밸런스 게임 🕵️‍♀️</h3>
- ~~~

<br/>

## 🗣️ 후기

>- 이득규: ~~~~

>- 홍주연: ~~~~

>- 배하은: ~~~~

>- 지동현: ~~~~

>- 박효찬: ~~~~


<br/>

## 🎃 웹 스크린 구성 및 기능

| **캐릭터 목록** |  **1:1 채팅 - 스폰지밥**  |  **1:1 채팅 - 버즈** |
| :---:|:---:|:---:|
| <img align="center" alt="메인페이지" src="../img/메인.PNG" width="240px" /> | <img align="center" alt="" src="../img/" width="240px" /> | <img align="center" alt="" src="../img/" width="240px" /> |

| **1:1 채팅 - 리바이** |  **1:1 채팅 - 에스카노르 (낮)**  |  **1:1 채팅 - 에스카노르 (밤)** |
| :---:|:---:|:---:|
| <img align="center" alt="" src="../img/" width="240px" /> | <img align="center" alt="" src="../img/" width="240px" /> | <img align="center" alt="" src="../img/" width="240px" /> |

| **1:1 채팅 - 김전일** |  **1:1 채팅 - 플랑크톤**  |  **단체 채팅 (일반 질문)** |
| :---:|:---:|:---:|
| <img align="center" alt="" src="../img/" width="240px" /> | <img align="center" alt="" src="../img/" width="240px" /> | <img align="center" alt="" src="../img/" width="240px" /> |

| **단체 채팅 (특정 캐릭터 지목)** |  **1:1 채팅 - 플랑크톤**  |  **단체 채팅 (일반 질문)** |
| :---:|:---:|:---:|
| <img align="center" alt="" src="../img/" width="240px" /> | <img align="center" alt="" src="../img/" width="240px" /> | <img align="center" alt="" src="../img/" width="240px" /> |
