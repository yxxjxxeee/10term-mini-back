# IndukToon Backend

개발 기간: 2025.07 ~ 2025.08

모던 애자일 10기 미니 프로젝트로 진행한 네이버 웹툰 클론 코딩 "인덕툰(IndukToon)"의 백엔드 리포지토리입니다.<br/>
요일별 웹툰 목록 조회, 에피소드 열람, 별점 / 댓글 / 즐겨찾기 등 네이버 웹툰의 핵심 기능을 클론 구현했습니다.<br/>
회원가입 / 로그인, Access / Refresh Token 기반 인증, 닉네임 / 비밀번호 변경 등 회원 기능도 함께 제공합니다.

## Tech Stack

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=jsonwebtokens)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Traefik](https://img.shields.io/badge/Traefik-24A1C1?style=for-the-badge&logo=traefikproxy&logoColor=white)

## 서비스 화면

| 메인 | 로그인 |
|---|---|
| <img width="100%" src="https://github.com/user-attachments/assets/8b20ebad-a25f-4999-9fc1-f431cce91da2" /> | <img width="100%" src="https://github.com/user-attachments/assets/8ef69262-b8ff-4206-a842-1f440973456c" /> |

| 관심목록 | 마이페이지 |
|---|---|
| <img width="100%" src="https://github.com/user-attachments/assets/d8cf5932-e08a-4326-b5c6-1b6fe19cd6d8" /> | <img width="100%" src="https://github.com/user-attachments/assets/0d044ad8-9c0f-4eb8-8c72-9e657111db2e" /> |

| 웹툰 상세 | 검색 결과 |
|---|---|
| <img width="100%" src="https://github.com/user-attachments/assets/b0ab0f14-a802-4394-8bae-cfa11b15e757" /> | <img width="100%" src="https://github.com/user-attachments/assets/3c5ce261-de56-4326-95ed-70622e53db92" /> |

## System Architecture

<img width="2397" height="1164" alt="image" src="https://github.com/user-attachments/assets/8ed2e329-8455-4768-916d-0ce1b39ed14b" />

- 요청 흐름: `Client` → `Traefik (Reverse Proxy / TLS)` → `Express (Node.js)` → `MySQL`
- 인프라: `Docker Compose` (Traefik & App 컨테이너), Let's Encrypt 인증서 적용

## ERD

<img width="1770" height="720" alt="인덕툰(induktoon)" src="https://github.com/user-attachments/assets/6a67009f-7dd0-4510-9d81-1049f9b5d272" />

## Members

<table>
  <tr>
    <td align="center" width="200px">
      <img src="https://github.com/yxxjxxeee.png" width="120px" /><br/>
      윤지은<br/>
      <b>yxxjxxeee</b><br/>
      <a href="https://github.com/yxxjxxeee">@yxxjxxeee</a>
    </td>
    <td align="center" width="200px">
      <img src="https://github.com/dlehdhun.png" width="120px" /><br/>
      이동훈<br/>
      <b>dlehdgns</b><br/>
      <a href="https://github.com/dlehdhun">@dlehdhun</a>
    </td>
  </tr>
</table>
