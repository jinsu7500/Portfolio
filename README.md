# Portfolio
-------------------

+ 이름 | 박진수 (Jisnu Park)
+ 나이 | 1997년생
+ 학력 | 공주대학교 컴퓨터공학부 컴퓨터공학전공
+ 개발이력

  + [(2021) Reminder Calendar 개발 - JavaScript](#ReminderCalendar)  
  <게임>
  + [(2019) 퍼즐게임 SemanticTravel 코딩 개발참여](#SemanticTravel)
  + [(2021) 3D 미로찾기게임 MazeGame 1인개발](#MazeGame)
  + [(2021) 3D 장애물 달리기게임 Shotgun 개발 팀리더](#ShotGun)
  + [(2021) 2D 실시간 협동 퍼즐게임 BreakFriendShip 개발 팀리더](#BreakFriendShip)
-----------------------------------------
## ReminderCalendar
### 프로젝트 소개
알람을 설정해두면 정해진 시간에, 음악이 재생되는 웹 어플리케이션  

### 개발방향
다양한 정보를 한눈에 쉽게 알아볼 수 있도록, 가독성과 간결성을 중요시 하였다.  
### 프로그램 기능  
+ 날짜 선택  
![image](https://user-images.githubusercontent.com/56360477/135053390-9b9604a9-1ac7-4c7a-8713-72244e76be7a.png)  
  
+ 달력출력  
![image](https://user-images.githubusercontent.com/56360477/135053423-caf1a197-5e02-480b-86c3-43b489defde8.png)  

+ 일정 추가  
![image](https://user-images.githubusercontent.com/56360477/135053458-9395e9a1-0867-4335-814e-1530bba6749a.png)  

+ 현재시간 및 오늘의 일정 출력  
![image](https://user-images.githubusercontent.com/56360477/135053504-8d0f8ed9-924a-43a4-adac-a3ca679799b4.png)  

+ 알람설정  
![image](https://user-images.githubusercontent.com/56360477/135053710-94b15e30-7885-4389-80f9-e201a76e4828.png)  


### 실행화면  
![image](https://user-images.githubusercontent.com/56360477/135053758-b4e01571-31c9-4ffa-8773-991091f3373b.png)  



-----------------

## SemanticTravel

### 프로젝트 소개
Unity를 활용하여 2D 모바일 점프게임이다. 플레이어는 여러 블럭들을 통과하여 상위 스테이지로 향해야 한다.

* 개발버전 Unity3d 2019.2.6f1

### 기능
* 플레이어 이동 : 휴대폰의 중력센서를 활용하여, 좌,우로 이동할수 있다. 
* 점프 : 스마트폰의 터치치, 플레이어가 점프를 한다.
* 사망 : 플레이어가 추락시, 사망, Retry 버튼이 출력된다.

### 게임 소개

![image](https://user-images.githubusercontent.com/56360477/144377024-45ec2bf2-ecbf-4689-b7c4-33fa5c63b15f.png)

게임 시작화면, 터치시 게임이 시작한다.


![image](https://user-images.githubusercontent.com/56360477/144377107-8e40a99d-4aa6-48be-9f08-83a4273723d0.png)

기본블록


![image](https://user-images.githubusercontent.com/56360477/144377161-c9a7fc64-7f3d-418b-b77a-0ae62c50ba2a.png)

좌우 이동 블록


![image](https://user-images.githubusercontent.com/56360477/144377335-152c4ef7-4bdd-406b-bb6b-cd26dcde5cd1.png)

상하 이동 블록

![image](https://user-images.githubusercontent.com/56360477/144377452-8c60440a-3c48-4eeb-8c58-74ee02097db0.png)

Break 블록, 블록위에 플레이어가 위치시, 일정시간 이후 블록이 사라진다.


![image](https://user-images.githubusercontent.com/56360477/144377621-0bc99cf2-74a0-458d-ae3c-ec4c90ad01ec.png)

게임이 시작되면 블록들이 랜덤으로 생성된다.


![image](https://user-images.githubusercontent.com/56360477/144377806-7370627b-6c2b-4af3-875a-ed9465ff0756.png)

도착블록 도달시, 다음스테이지로 넘어간다.

### 소스코드
https://github.com/KimSoo-hwan/SemanticTravel


-----------------------------------------

## MazeGame
### 프로젝트 소개

Unity3D를 활용한 1인 게임 개발 프로젝트이다.
단순하지만 플레이하는 재미가 있는 퍼즐장르의 게임을 개발하고자 하였다.

MazeGame은 미로찾기에 퍼즐요소를 합친 게임,
1인칭으로 개발함으로써 플레이어는 실제 미로를 탐험하는 느낌을 받을 수 있을 것이다.


### 기능

* 플레이어 이동 : 플레이어는 W,S,A,D키를 사용하여 전,후,좌,우로 이동할 수 있다.
* 카메라 회전 : 마우스 이동을 통해 카메라 시점을 회전시킬 수 있다.
* 상호작용 기능 : G키를 사용하여, 플레이어와 오브젝트간의 상호작용이 가능하다.
* 미로생성 기능 : 깊이 탐색 알고리즘(DFS)을 사용하여 게임을 실행할 때 마다 새롭게 미로를 생성한다.
  * DFS 알고리즘
  1) 미로는 접근이 불가능한 구역이 존재해서는 안된다. 즉, 모든 셀이 탐색가능해야 한다는 전제조건이 있다.
  2) 20 by 20의 바둑판 모양의 격자모양 셀을 생성
  3) 랜덤으로 하나의 셀을 지정, 방문기록을 한다.
  4) 선택된 셀의 인접한 셀들 중, 방문기록이 없는 셀을 찾는다.
  5) 방문하지 않은 셀들 중 하나를 선택, 사이의 벽을 제거하고 방문기록을 한다.
  6) 4~5번의 과정을 모든 셀을 방문 할 때까지 반복한다.


  



### 프로그램 구조도 및 흐름

![image](https://user-images.githubusercontent.com/56360477/135048201-71aa3328-f740-4643-994c-83dd9f3451cf.png)

![image](https://user-images.githubusercontent.com/56360477/135048224-9db0f9c7-fb4f-422f-9796-e58a91e340b0.png)


### 조작법

W : 앞으로 이동
S : 뒤로 이동
A : 왼쪽으로 이동
D : 오른쪽으로 이동
G : 오브젝트 상호작용
마우스이동 : 카메라회전


### 실행화면
![타이틀화면](https://user-images.githubusercontent.com/56360477/135048628-30eb7a8a-c512-420d-81f5-b132ac6ce6f9.gif)

![튜토리얼](https://user-images.githubusercontent.com/56360477/135048631-330c971c-be14-4889-b295-0410f3a90e8c.png)

![미로맵 움직임](https://user-images.githubusercontent.com/56360477/135048592-d04bd5ee-e7d1-4069-b2e7-940471b2ddc4.gif)

![복도](https://user-images.githubusercontent.com/56360477/135048608-7b88e74e-8c86-4c8b-a329-440ffa70ae61.gif)

![사망](https://user-images.githubusercontent.com/56360477/135048610-1fd8ddd9-507d-4c83-b636-b73649893c78.gif)

![엘레베이터](https://user-images.githubusercontent.com/56360477/135048616-f186160f-d709-4195-b6b0-653b2b24f104.gif)

![큐브](https://user-images.githubusercontent.com/56360477/135048619-b725987e-c953-4273-8dca-8ae151596b37.gif)

![큐브발판](https://user-images.githubusercontent.com/56360477/135048622-d42ccfdc-8ad5-4d6f-8755-772c0969deac.gif)

![큐브픽업](https://user-images.githubusercontent.com/56360477/135048624-c5f76af2-9390-4842-932d-6021805ef764.gif)

![퍼즐맵3](https://user-images.githubusercontent.com/56360477/135048657-e3f22fb5-ee47-4c47-b67f-02ec3ab10e5b.gif)

![회전](https://user-images.githubusercontent.com/56360477/135048667-db567a4c-d755-480e-88a9-ba2825a050f5.gif)

![퍼즐 올클리어](https://user-images.githubusercontent.com/56360477/135048633-b7c892d5-abee-45e2-8cc0-0ff9d825a6a7.gif)



### 소스코드 
https://github.com/jinsu7500/21_1_MAZEGAME


----------------
## ShotGun

### 프로젝트 소개

3인 팀프로젝트로서 개발한 장애물 달리기 게임이다.
각각의 팀원이 하나의 스테이지를 맡아 개발하였으며, 본인은 플레이어,1스테이지(숲)을,UI,BGM 등을 담당하여 개발하였다.

SHOTGUN은 유니티3D 엔진을 활용한 장애물 달리기 게임이다. 

게임 AutoSaveGame-"ALT F4"와, 예능프로그램 "출발 드림팀"을 모티브로하여, 개발하였다.
플레이어는 맵에 배치된 다양한 장애물을 통과하여 골인지점에 도달해야한다.


### 게임 스토리

![image](https://user-images.githubusercontent.com/56360477/135045871-b4135e62-67b8-427a-8c0f-8af72074acb7.png)

게임의 주인공인 ‘Bandit’은 트레져헌터이다. 그는 어느날 숲속에 숨겨진 유적지에 엄청난 보물이 있다는 소식을 듣게 된다. 그는 보물을 찾기위해 거대한 숲으로 들어갔다. 숲속에는 누군가 설치한 온갖 함정들이 존재하였는데, 그는 이러한 함정들을 헤쳐나가며, 보물을 찾기 위해 노력한다.

### 프로그램 구조


![image](https://user-images.githubusercontent.com/56360477/135045982-f927759f-bc28-4bf8-939c-c39e66eac0af.png)



### 조작법

W:위로 이동
S:아래로 이동
A:왼쪽으로 이동
D:오른쪽으로 이동
SPACEBAR:점프
SHIFT:달리기
ESC:메뉴


### 실행화면

![image](https://user-images.githubusercontent.com/56360477/135046246-cae84118-1052-46b4-9954-efad41fb8465.png)
![image](https://user-images.githubusercontent.com/56360477/135046262-05e5fae7-dfaf-4c08-9518-102d615f4692.png)
![image](https://user-images.githubusercontent.com/56360477/135046275-c1d67f73-13b1-4ae3-a128-470932bd07a4.png)
![image](https://user-images.githubusercontent.com/56360477/135046287-2ba0b7b0-4083-4a44-8b6c-6aa866adb1aa.png)
![image](https://user-images.githubusercontent.com/56360477/135046296-741374cb-b366-495b-aad2-bb880fff692e.png)
![image](https://user-images.githubusercontent.com/56360477/135046307-818ae03d-0a77-4985-bf5b-87e0c6627b26.png)



### 시연영상

https://www.youtube.com/watch?v=OlFlbu8n1_M


### 소스코드
https://github.com/jinsu7500/SHOTGUN

--------------------
## BreakFriendShip

### 프로젝트 소개  
3인 팀프로젝트로서, Unity3D의 Photon,PlayFab등을 활용하여 개발한 2D멀티 퍼즐 게임이다. 본인은 캐릭터, 맵,UI,사운드, 스테이지등을 담당하여 개발하였다.

BreakFriendship은 유니티엔진을 활용한 실시간 협동 2D 플랫포머 멀티게임이다. 최대 4인의 플레이어가 실시간으로 게임에 참여하며, 플랫폼(발판)위를 뛰어다니는 점핑 액션 게임이다. 유사프로그램으로는 "닌텐도"사의 슈퍼마리오 브라더스, "Pixel"사의 "ClaveStory" "TecoPark"사의 "Pico Park"등이 있다.

개발 플랫폼은 PC Window이며 개발환경은 "Unity3d 2020.3.8f1"버전을 사용하였다.

### 프로젝트 추친 일정
![image](https://user-images.githubusercontent.com/56360477/147561040-f0fcf13f-e60f-40b5-9756-1b7d421d9546.png)

프로젝트 개발의 총 기간은 7주이다.  

### 주요 기술
+ Unity3d
+ C#
+ PlayFab
+ Photon Cloud
+ GitHub

### 프로그램 동작도
![image](https://user-images.githubusercontent.com/56360477/147561307-b5bf8112-6274-4f18-b473-8ad67ab1c490.png)

1. 회원가입 - 데이터 분석, 스토리지, 처리 및 내보내기를 위한 도구 세트인 PlayFab을 프로젝트에
적용시켜 이메일, 닉네임, 비밀번호를 PlayFab에 저장시킨다.
2. 로그인 - 데이터 분석, 스토리지, 처리 및 내보내기를 위한 도구 세트인 PlayFab을 프로젝트에
적용시켜 저장된 닉네임을 불러온다.
3. 캐릭터 선택 - 4가지 캐릭터가 존재하고 플레이어는 선택한 캐릭터로 게임을 진행하게 된다.
4. 로비접속 - Photon서버에 접속을 하여, 방생성, 또는 생성된 방에 게임참가를 할 수 있다.
5. 방 생성 - 플레이어가 방 생성을 하게 되면, 방 인원수를 2~4명까지 선택 할 수 있고 선택한 인원수에
맞는 방에 적용된다.

6. 방 접속 - 방 접속을 하게 되면 접속한 플레이어의 캐릭터, 닉네임, Ready 텍스트가 플레이어 마다
생성된다. Ready버튼을 누르게 되면 누른 플레이어의 Ready 텍스트가 빨간 색으로 변하게 된다. 접속한
플레이어끼리 실시간 소통할 수 있는 채팅방이 있다.
7. 1~6라운드, 총 6개의 라운드가 존재하며, 각각의 라운드마다 특색있는 퍼즐요소를 추가하여 플레이어들이 목표 위치에 도달하면 클리어하도록 설정하였다.


### 프로그램 기능
![image](https://user-images.githubusercontent.com/56360477/147561430-384b0bd8-9512-494e-901a-d6e951438254.png)  

### 조작법
+ ← 키보드 방향키 : 좌측이동 
+ → 키보드 방향키 : 우측이동
+ Space : 점프,더블점프

### 프로그램 실행결과
+ 타이틀 화면  
![image](https://user-images.githubusercontent.com/56360477/147561724-81514e8b-fb72-407f-80e4-7692cce5b921.png)  
  - Start버튼으로 게임을 시작 할 수있고, Exit버튼으로 게임을 종료 할 수 있다.

+ 로그인 화면  
![image](https://user-images.githubusercontent.com/56360477/147562089-6c10a251-7074-4b6f-8c86-3a1023974b4f.png)  
  - 회원가입 버튼 클릭시 가입페이지로 이동한다. PlayFab과 연동되어 유저데이터를 저장 및 불러온다.

+ 캐릭터 선택 화면  
![image](https://user-images.githubusercontent.com/56360477/147562216-1e9a3720-0622-4235-9d27-c13014a3b4ef.png)  
  - 4가지의 캐릭터중 한가지를 선택할 수 있다.  

+ 로비 화면  
 ![image](https://user-images.githubusercontent.com/56360477/147562507-b63d97ea-33ae-400d-a417-a1570f4f82ec.png)  
   -  로비에서는 현재 접속한 유저의 수와, 플레이중인 방을 보여준다. 방이름을 설정하고 Create버튼 클릭시 방을 만들수 있고, QuickStart버튼을 클릭할 시 현재 있는 방들중 하나에 랜덤으로 입장하게 된다.

+ 방 화면  
  ![image](https://user-images.githubusercontent.com/56360477/147562626-6d41bcf3-2e75-4efc-bc7f-796bc72698a2.png)  
  -  현재 접속한 플레이어와, 플레이어의 레디상태를 표시해준다. 플레이어간의 실시간 채팅이 가능한 채팅창이 존재한다.  

+ 1Round - 튜토리얼  
![round1_resize](https://user-images.githubusercontent.com/56360477/147594686-7d607780-341b-45e3-b79d-956f793b3049.gif)  


+ 2Round - 총알피하기   
![round2_resize](https://user-images.githubusercontent.com/56360477/147594693-976fe2ad-3c59-4944-abe6-c414ab936ab5.gif)   

+ 3Round - 무궁화 꽃이 피었습니다.  
  ![round3_resize](https://user-images.githubusercontent.com/56360477/147594801-84bdd18d-ed2c-402f-b3e8-83dac9a1b3fa.gif)  
  
+ 4Round - 일심동체 유령조작  
![round4_resize](https://user-images.githubusercontent.com/56360477/147594869-9a80b8c9-ea34-4f98-8f9e-7fd7c05ec1fb.gif)  

+ 5Round - 장애물 피하기  
 ![round5_resize](https://user-images.githubusercontent.com/56360477/147594931-7f4ef75e-310e-4e32-a221-e6881a4dcd64.gif)  


+ 6Round - 추적 몬스터 피하기  
![round6_resize](https://user-images.githubusercontent.com/56360477/147594937-03454d7a-78a9-4846-a757-e7caa36a1afb.gif)  



### 시연영상
https://www.youtube.com/watch?v=91RTeFIy7q4

### 소스코드
https://github.com/jinsu7500/BreakFriendship

----------------------





