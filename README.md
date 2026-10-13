# Log Watchdog — 기획 문서 사이트

MMORPG 로그 정제와 봇 · 작업장 탐지 팀 프로젝트의 문서 모음입니다.

| 페이지 | 대상 | 내용 |
|---|---|---|
| `index.html` | 모두 | 문서 안내, 진행 방식, 한 장 요약 |
| `plan.html` | 우리 팀 | 1차 · 팀 기획서 (3인 · 3일) |
| `request.html` | 데이터 팀 | 2차 · 데이터 요청서 |
| `appendix-a.html` | 모두 | 별첨 A · 실제 데이터 출처와 기업 공개 대회 |
| `appendix-b.html` | 모두 | 별첨 B · 출처별 원문 번역 정리 |

PDF는 `downloads/`, 요약 이미지는 `assets/summary.png`에 있습니다.

## GitHub Pages로 배포하기

1. GitHub에서 새 저장소를 만듭니다 (예: `log-watchdog-docs`, Public).
2. 이 폴더 안의 파일 전체를 저장소 최상위에 올립니다. `.nojekyll` 파일도 함께 올려야 합니다.
   ```bash
   git init
   git add .
   git commit -m "docs: 기획 문서 사이트"
   git branch -M main
   git remote add origin https://github.com/<계정>/log-watchdog-docs.git
   git push -u origin main
   ```
3. 저장소 **Settings → Pages**에서 Source를 `Deploy from a branch`, Branch를 `main` / `/ (root)`로 지정하고 저장합니다.
4. 1~2분 뒤 `https://<계정>.github.io/log-watchdog-docs/`에서 열립니다.

외부 라이브러리나 빌드 과정 없이 HTML · CSS만으로 되어 있어 그대로 동작합니다. 한글 글꼴은 보는 사람 PC의 기본 글꼴(Noto Sans KR, 맑은 고딕 등)을 씁니다.
