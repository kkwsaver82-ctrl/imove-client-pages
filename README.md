# 아이무브 고객 관리 페이지 - Codex 작업용 소스

이 폴더는 ChatGPT와 함께 만든 아이무브 아동 운동발달 관리 페이지의 현재 소스 모음입니다.
Codex, Claude, GPT, 로컬 브라우저에서 이어서 수정할 수 있도록 구성했습니다.

## 파일 구조

```text
imove_client_pages_codex/
├─ src/
│  ├─ original_claude_template.html          # 사용자가 처음 제공한 Claude 원본 템플릿
│  ├─ client_management_page_full.html       # 확장형 고객 관리 페이지
│  ├─ client_management_page_simplified.html # 관리코드/버튼 제거, 기본정보 축소 버전
│  ├─ client_management_page_overview.html   # 전체 페이지가 한눈에 보이도록 축소 구성한 버전
│  ├─ live_html_editor_fixed.html            # 좌측 코드 / 우측 실시간 미리보기 편집기
│  ├─ live_html_editor_simplified.html       # simplified 페이지가 들어간 편집기
│  └─ live_html_editor_overview.html         # overview 페이지가 들어간 편집기
├─ screenshots/
│  ├─ 01_broken_preview.png
│  ├─ 02_fixed_editor_preview.png
│  ├─ 03_command_input_example.png
│  ├─ 04_client_page_partial_preview.png
│  └─ 05_two_windows_example.png
└─ docs/
   ├─ CODEX_TASKS.md
   └─ PRIVACY_GUIDE.md
```

## 현재 권장 기준 파일

- 고객에게 보낼 페이지 기준: `src/client_management_page_overview.html`
- GPT/Claude와 좌우 편집하며 확인할 파일: `src/live_html_editor_overview.html`
- 원본 참고: `src/original_claude_template.html`

## 운영 원칙

1. 고객별 파일은 실명 대신 코드 사용 권장: 예) `IM-2026-001.html`
2. 고객에게 보내는 파일에는 버튼/관리 기능을 숨기고, 보호자 안내용 정보만 남긴다.
3. 사진, X-ray, 평가표를 넣을 경우 이름, 생년월일, 병원번호, 촬영번호를 가린 뒤 사용한다.
4. GitHub Pages 공개 배포는 개인정보 보호 측면에서 권장하지 않는다.
5. 여러 고객용으로 복사할 때는 `CLIENT_DATA` 영역만 바꾸는 방식을 유지한다.

## Codex에게 줄 첫 명령 예시

```text
이 저장소는 아이무브 아동 운동발달 관리 페이지 프로젝트입니다.
현재 기준 파일은 src/client_management_page_overview.html 과 src/live_html_editor_overview.html 입니다.
디자인 톤은 유지하고, CLIENT_DATA 영역만 쉽게 수정할 수 있는 구조를 유지해 주세요.
먼저 파일 구조를 파악하고 README.md와 docs/CODEX_TASKS.md를 읽은 뒤, 개선 계획을 제안해 주세요.
```
