# 🎹 InMusic
> **Photon Fusion 2 기반 1:1 멀티플레이 리듬 게임**

**InMusic**은 사용자의 Steam 정보를 연동하여 실시간으로 다른 사용자와 대결할 수 있는 멀티플레이 리듬 게임입니다. 단순한 게임 구현을 넘어 클라이언트-서버 아키텍처와 데이터 동기화 등 기술적 외연 확장에 집중한 프로젝트입니다.

## 🚀 주요 기능 (Key Features)

- **실시간 1:1 멀티플레이**
  - **Photon Fusion 2 (Shared Mode)** 를 활용하여 P2P 방식의 안정적인 네트워크 환경을 구축했습니다.
  - **RPC(원격 프로시저 호출)** 및 **네트워크 변수([Networked])** 동기화를 통해 노트 판정, 게임 시작, 플레이어 상태 등을 실시간으로 처리합니다.
- **Steam API 연동**
  - **Steamworks.NET**을 사용하여 별도의 가입 없이 Steam 닉네임과 ID를 자동으로 가져와 사용자 프로필을 생성합니다.
- **백엔드 데이터 관리**
  - **Xampp(PHP + MySQL)** 환경을 구축하여 사용자의 플레이 기록(Score, Accuracy 등)을 DB에 저장하고 관리합니다.
  - 클라이언트와 서버 간 데이터 교환은 **JSON** 형식을 사용하며, 비동기 처리를 통해 UI 반영 시 끊김 없는 사용자 경험을 제공합니다.
- **동적 음악 리소스 관리**
  - 경로 기반으로 **BMS(Be-Music Source) 파일**을 파싱하여 노트 데이터를 생성하며, 앨범 아트 및 오디오/비디오 프리뷰 기능을 지원합니다.
  - **무한 스크롤 UI**를 구현하여 많은 양의 음악 목록을 효율적으로 탐색할 수 있습니다.
## 🛠 개발 환경 및 기술 스택 (Tech Stack)

- **Engine**: Unity
- **Language**: C# (Client), PHP (Backend)
- **Database**: MySQL (Xampp)
- **Networking**: Photon Fusion 2
- **External API**: Steamworks.NET (Steam API)
- **Design**: Figma (UI/UX 설계)

## 🕹 조작 방법 (Controls)

- **방향키 / Enter**: 메뉴 이동 및 선택
- **D, F, J, K**: 리듬 게임 노트 입력 (4키 방식)
- **F1**: 키 가이드 표시
- **F10**: 옵션 설정

## 👥 팀 구성 및 역할 (동의대학교 창업동아리 'Insight')

- **총 규모**: 팀당 약 2.5인 구성의 2개 팀 협업
- **주요 역할 (본인 파트 포함)**:
  - **Team 1**: 메인 로비, 키 설정/가이드 UI 시스템 구현
  - **Team 2**: 음악 목록 시스템, 멀티플레이 대기방 및 결과창, 스팀 API 연동, 백엔드(PHP/SQL) 구축

## 🔗 관련 링크 (Links)

- **Demo Video**:
  - [싱글 플레이 시연](https://youtu.be/JRYU3J4ES2w)
  - [멀티 플레이 시연](https://youtu.be/DxBgg7xzQq4)
- **Design**: [Figma UI 디자인안](https://www.figma.com/design/85ut1knreVE222dAx5zELe/%EB%A6%AC%EB%93%AC%EA%B2%8C%EC%9E%84?node-id=0-1)
