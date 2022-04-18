# Do it! 클론코딩줌 코딩 베타 테스트
이지퍼블리싱 - Do it! 클론코딩줌 코딩 베타 테스트


## 프로젝트명 : Noom

- Zoom Clone using NodeJS, WebRTC and Websockets.

### 베타 테스트 기간
- 2022년4월14일 ~ 2022년4월21일

### 테스트 환경

- Os : Mac Os , M1 Pro
- Tool : Intellij
- Server : Node.js
- View Engine : Pug
- Css Framework : MVP.css
- PC Browser : Chrome, Safari
- Mobile Browser : Chrome, Safari

### 목차
01 : 줌클론코딩시작하기
- 1 클론코딩Zoom,이런기능을만들어요! 01-2 클론 코딩 수업 준비하기
- 3 코드 셋업 1: 프로젝트 생성
- 4 코드 셋업 2: 서버
- 5 코드 셋업 3: 프런트엔드

02 : 웹소켓을 이용한 실시간 기능 구현하기
- 1 HTTP vs 웹소켓
- 2 웹소켓 설치하고 서버 만들기 02-3 웹소켓 이벤트
- 4 메시지 주고받기

03 : 실시간 채팅 완성하기
- 1 채팅 기능 준비하기 
- 2 사용자 간 채팅하기 
- 3 닉네임 추가하기 1 
- 4 닉네임 추가하기 2

04 : socket.io를 이용한 채팅룸 만들기
- 1 socket.io 설치하기
- 2 socket.io 다루기
- 3 채팅룸 만들기
- 4 채팅룸 안에서 메시지 교환하기 04-5 채팅룸 알람 보내기

05 : 채팅룸 완성하기
- 1 닉네임 추가하기
- 2 채팅룸 관리하기
- 3 사용자 수 표시하기 05-4 Admin panel 사용하기

06 : 화상 채팅 준비하기
- 1 카메라 불러오기
- 2 비디오와 오디오 제어하기 
- 3 카메라 변경하기

07 : 화상 채팅 완성하기
- 1 WebRTC 알아보기
- 2 채팅룸 만들고 관리하기
- 3 데이터 교환을 위한 offer 보내기 
- 4 offer에 응답하는 answer 보내기
- 5 peer-to-peer 연결 생성하기
- 6 미디어 트랙 제어하기
- 7 메시지 교환 기능 추가하기

08 : 스타일시트 추가하기
- 1 스타일 정의를 위한 준비
- 2 스타일 정의하기

### 점검 사항

pug
    - 들여쓰기를 제대로하지 않으면 에러가 자주 발생

07 : 대화 상대의 미디어 출력하기
- Chrome to Chrome
  - 내 화면 및 상대방 화면 출력 잘됨.
  - 상대방이 나가면 상대방의 마지막 화면이 남아서 사라지지 않음
- Chrome to Safari
  - 크롬에서는 내 화면 및 상대방 화면 출력 잘됨.
  - 사파리에서는 내 화면만 출력 상대방 화면 출력되지 않음.
  - 크롬에서 상대방이 나가면 상대방의 마지막 화면이 남아서 사라지지 않음
- Safari to Safari
  - 내 화면은 잘 출력되지만, 상대방 화면은 출력되지음.
  - 이와 동시에 상대방이 채팅방 접속시 내 화면이 "카메라끔" 으로 설정된거 같이 검게 변하함.

07 : 모바일에서 실행하기, STUN 서버
- Mobile to Mobile
  - Chrome to Chrome
    - 내 화면은 잘 출력되지만, 상대방 화면은 출력되지음.
  - Chrome to Safari
    - 내 화면은 잘 출력되지만, 상대방 화면은 출력되지음.
  - Safari to Safari
    - 내 화면은 잘 출력되지만, 상대방 화면은 출력되지음.

- pc to Mobile
  - Chrome to Chrome
    - 같은 와이파이 환경에서 pc의 내 화면과 상대방 화면은 잘 출력되지만 모바일에서
      상대방 회면이 나타나지 않음.
    - 와이파이가 아닌 lte 또는 5g 내 화면은 잘 출력되지만, 상대방 화면은 출력되지음.
    
  - Chrome to Safari
    - 같은 와이파이 환경에서 pc의 내 화면과 상대방 화면은 잘 출력되지만 모바일에서
      상대방 회면이 나타나지 않음.
    - 와이파이가 아닌 lte 또는 5g 내 화면은 잘 출력되지만, 상대방 화면은 출력되지음.
    
  - Safari to Safari
    - 와이파이 환경이거나 lte, 5g 환경에서 내 화면은 잘 출력되지만, 상대방 화면은 출력되지음.

### 소감

예전부터 니꼬쌤 강의와 유튜브를 즐겨 보고 있었습니다. 아직 들어보지 못한 강의가 많았는데, 그중에 하나가 "줌 클론 코딩" 이었습니다.
바쁜 생활 속에서 계속 관심만 있던 강의를 이렇게 책으로 출간한다는 소식에 냉큼 베타테스터를 신청하게 되었습니다.

개인적으로는 node.js에 관심이 많았고 코로나 시기 전부터 "webRTC"에 대한 관심이 많았기 때문에 한 번은 토이 프로젝트로 진행해 보고 싶은 주제였습니다.
그리고 니꼬쌤 강의를 들어보신 분들은 아시겠지만, 책의 문장 자체가 마치 니꼬쌤 강의를 보는 듯은 느낌을 받았습니다. 그래서 책을 보는 게 상당히 편했습니다.
이 책에서는 "pug"라는 뷰 엔진이라는 걸 처음 사용했는데, 종종 들어봤던 언어라서 기존 HTML 과 어떻게 다른지 경험해 볼 수 있는 기회였습니다.
웹 개발에 대한 개념이 전혀 없다면 다소 버거울 수도 있겠지만, 그래도 책의 내용 자체가 따라 하기 어렵게 구성되어 있지는 않아서
초보 개발자분들도 충분히 책만 잘 보고 따라 하면 문제없이 진행이 가능할 거 같습니다. 

종종 개발 관련 서적을 보면서 따라할때 어떤 코드를 삭제해야하고 어떤 코드를 추가해야하는지 명확하게 보여주지 않고 변경이 완료된 코드만 보여주는 경우가많은데
이 책에서는 기존 코드에서 삭제해야할 부분과 추가해야할 부분이 명확해서 따라하기 참 편하다는 느낌을 받았습니다.

이 책만으로도 충분하겠지만 이해가 좀 부족하다 싶으면 니꼬쌤 "줌 클론 코딩" 강의도 같이 보면 좋을 거 같습니다! 적극 추천합니다.
그리고 저에게는 이 책과 더블어 니꼬쌤 강의와 유튜브가 많은 도움이 되었습니다. 더 많은 초보 개발자분들이 도움을 받았으면 좋겠습니다.
또한 니꼬쌤 강의 책에 조금이나마 기여할 수 있는 이렇게 좋은 기회를 주신 담당자분께 감사드립니다.
테스트 진행하면서 완성된 소스코드는 제 깃허브 "https://github.com/m-veloper/beta-test-zoom-clone" 올려두었습니다.








