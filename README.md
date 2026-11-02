# SSAG Lab 홈페이지 (Quarto + GitHub Pages)

주소: https://manjukcus.github.io

## 파일 구성

| 파일 | 내용 |
|---|---|
| `_quarto.yml` | 사이트 제목, 상단 메뉴, 하단 문구 |
| `index.qmd` | Home (소개, 학력, 지도) |
| `news.qmd` | News |
| `research.qmd` | Research (연구 관심사) |
| `papers.yml` | 논문 목록 데이터. Research 페이지에 연도순으로 자동 표시 |
| `teaching.qmd` | Teaching |
| `styles.scss` | 글꼴, 색, 레이아웃 |
| `papers.ejs` | 논문 목록 표시 형식 (보통 고칠 일 없음) |
| `images/` | 그림 파일 |

## 바꿔 넣어야 할 그림

`images/research/` 의 그림은 자리표시용입니다. 같은 파일 이름으로 덮어쓰면 됩니다.

| 파일 | 논문 |
|---|---|
| `2025-pg.png` | The Professional Geographer (2025) |
| `2024-cir.png` | Child Indicators Research (2024) |
| `2023-ijgis.png` | IJGIS (2023) |
| `2022-gean.png` | Geographical Analysis (2022) |
| `2018-kaeg.png` | 한국경제지리학회지 (2018) |
| `2017-kaug.png` | 한국도시지리학회지 (2017) |

## 자주 하는 수정

- 새 소식: `news.qmd`에서 연도 아래 맨 위에 날짜 한 줄, `:   내용` 한 줄을 추가
- 새 논문: `papers.yml`에서 항목 하나를 복사해 붙이고 내용만 수정 (그림은 `images/research/`에)

## 수정 후 게시하는 순서

1. VS Code 터미널에서 `quarto preview` 로 확인
2. 소스 제어 탭에서 커밋 후 동기화(push)
3. 터미널에서 `quarto publish gh-pages`
