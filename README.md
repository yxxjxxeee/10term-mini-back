# IndukToon

> 네이버 웹툰의 핵심 기능을 구현한 웹툰 클론 서비스

모던 애자일 10기 미니 프로젝트로 진행한 인덕툰(IndukToon)의 백엔드 리포지토리입니다.<br/>
요일별 웹툰 조회부터 회차 열람, 별점, 댓글, 관심 웹툰, 사용자 인증 기능을 제공합니다.

## 팀원

<table>
  <tr>
    <td align="center" width="200px">
      <a href="https://github.com/yxxjxxeee">
        <img src="https://github.com/yxxjxxeee.png" width="120px" alt="윤지은" />
      </a>
    </td>
    <td align="center" width="200px">
      <a href="https://github.com/dlehdhun">
        <img src="https://github.com/dlehdhun.png" width="120px" alt="이동훈" />
      </a>
    </td>
  </tr>
  <tr>
    <td align="center"><b>윤지은</b><br/><a href="https://github.com/yxxjxxeee">@yxxjxxeee</a></td>
    <td align="center"><b>이동훈</b><br/><a href="https://github.com/dlehdhun">@dlehdhun</a></td>
  </tr>
</table>

## 주요 기능

### 1. 요일별 웹툰 조회

요일별 웹툰 목록을 확인하고 관심순, 업데이트순, 조회순, 별점순으로 정렬할 수 있어요.

<img width="100%" src="https://github.com/user-attachments/assets/8b20ebad-a25f-4999-9fc1-f431cce91da2" alt="요일별 웹툰 목록" />

### 2. 웹툰 상세 및 회차 열람

웹툰 상세 정보와 회차 목록을 확인하고, 원하는 회차를 열람할 수 있어요.<br/>
회차별 조회 수와 별점, 댓글 및 대댓글도 함께 관리해요.

<img width="100%" src="https://github.com/user-attachments/assets/b0ab0f14-a802-4394-8bae-cfa11b15e757" alt="웹툰 상세 화면" />

### 3. 웹툰 검색

웹툰 제목이나 작가 이름으로 원하는 작품을 검색할 수 있어요.

<img width="100%" src="https://github.com/user-attachments/assets/3c5ce261-de56-4326-95ed-70622e53db92" alt="웹툰 검색 결과" />

### 4. 관심 웹툰

관심 있는 웹툰을 등록하고, 최신 등록순이나 업데이트순으로 모아볼 수 있어요.<br/>
여러 작품을 선택해 관심 목록에서 한 번에 삭제할 수도 있어요.

<img width="100%" src="https://github.com/user-attachments/assets/d8cf5932-e08a-4326-b5c6-1b6fe19cd6d8" alt="관심 웹툰 목록" />

### 5. 회원가입 및 로그인

회원가입과 로그인 후 Access Token과 Refresh Token을 이용해 안전하게 인증할 수 있어요.

<img width="100%" src="https://github.com/user-attachments/assets/8ef69262-b8ff-4206-a842-1f440973456c" alt="로그인 화면" />

### 6. 마이페이지

내 정보를 확인하고 닉네임과 비밀번호를 변경할 수 있어요.<br/>
관심 웹툰 목록도 마이페이지에서 바로 확인할 수 있어요.

<img width="100%" src="https://github.com/user-attachments/assets/0d044ad8-9c0f-4eb8-8c72-9e657111db2e" alt="마이페이지" />

## 기술 스택

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Traefik](https://img.shields.io/badge/Traefik-24A1C1?style=for-the-badge&logo=traefikproxy&logoColor=white)

## 시스템 아키텍처

- 요청 흐름: `Client` → `Traefik (Reverse Proxy / TLS)` → `Express (Node.js)` → `MySQL`
- 실행 환경: Docker Compose 기반 Traefik·애플리케이션 컨테이너 구성
- HTTPS: Let's Encrypt 인증서 자동 발급 및 갱신


<img width="2492" height="1050" alt="induktoon" src="https://github.com/user-attachments/assets/8a15803e-d81b-4306-b66c-1ca828644896" />
