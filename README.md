# 궤도 — 작은 우주 탐험

열 개의 질문으로 우주를 탐험하는 한국어 퀴즈 앱임당.
HTML, CSS, JavaScript, SVG가 모두 `index.html`에 들어 있으며,
외부 라이브러리나 네트워크 요청 없이 실행할 수 있는 정적 웹사이트임당.

## 주요 기능

- 문제마다 보기 4개, 정답마다 10점으로 총 100점 만점인 퀴즈임당.
- 정답·오답 피드백과 해설, 진행률, 최종 점수·정답률·이모지 반응을 제공하는 구성임당.
- 숫자키 `1`–`4`로 보기를 선택하고 `Enter`로 다음 문제로 이동하는 방식임당.
- 라이트·다크 테마, 키보드 포커스 표시, 동작 줄이기 설정을 지원하는 앱임당.

## 로컬 실행

저장소를 내려받은 뒤 `index.html`을 브라우저에서 직접 열면 되는 방식임당.
서버 실행, 빌드, 패키지 설치, 환경 변수 설정은 모두 불필요한 구성임당.

## GitHub Pages 배포

사이트 주소는 <https://Hyojin404.github.io/space-quiz/> 임당.

저장소의 **Settings → Pages → Build and deployment → Source**는
**GitHub Actions**로 설정해야 하는 구성임당.
배포 워크플로는 `.github/workflows/pages.yml`임당.

`main` 대상 PR에서는 `index.html`이 비어 있지 않은지 확인하고 게시 아티팩트를 준비하며,
실제 배포는 하지 않는 구성임당.
`main`에 변경이 반영되면 `index.html`만 GitHub Pages에 자동 배포하는 방식임당.
**Actions → GitHub Pages → Run workflow**에서 `main`을 선택해 수동 재배포도 가능한 구성임당.
배포 상태와 게시 URL은 해당 실행의 `Deploy to GitHub Pages` 작업에서 확인 가능한 정보임당.
