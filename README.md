# Tony's Sky View

드론으로 담은 제주와 여행지의 풍경, 영상·숏폼, 그리고 현장을 돕는 짧은 안내 페이지를 모아 둔 개인 웹 포트폴리오입니다.

## 이 저장소에 있는 것

| 구분 | 설명 |
|------|------|
| **Home** (`index.html`) | 메인 랜딩, 히어로 슬라이더, 대표 영상 소개 |
| **Places** (`places.html`, `places/`) | 명소·해안·지질 포인트별 안내 HTML |
| **Videos / Shorts** | 영상·숏폼 모음 페이지 |
| **Maps** (`maps.html`) | 지도 연동 콘텐츠 |
| **스타일** (`style.css`) | 공통 레이아웃·내비·히어로 등 |

`places/` 아래에는 예를 들어 갯깍 주상절리·해식동굴 안내(`Entablature.html`)처럼, 유튜브 설명란에 걸기 좋은 **지질·문화 보조 자료** 페이지도 포함되어 있습니다.

## 기술 스택

- 정적 HTML/CSS (서버 없이 GitHub Pages 등에 바로 올릴 수 있는 구성)
- [Tailwind CSS](https://tailwindcss.com/) (CDN)
- [Pretendard](https://github.com/orioncactus/pretendard), Google Fonts (Inter)
- 일부 페이지: Font Awesome, Noto Sans KR

## 로컬에서 보기

저장소 루트에서 `index.html`을 브라우저로거나, 간단한 정적 서버로 루트를 지정해 실행하면 됩니다.

```bash
# 예: Python 3
python -m http.server 8080
```

브라우저에서 `http://localhost:8080/` 로 접속합니다.

## GitHub Pages 배포 시 참고

- 사이트가 **저장소 URL**(`https://사용자명.github.io/저장소명/`)으로 열릴 때, 이미지·CSS 경로는 **루트 절대 경로**(`/images/...`)나 저장소명을 박은 경로(`/저장소명/images/...`)보다 **HTML 기준 상대 경로**(`./images/...`, `../images/...`)가 안전합니다. `places/` 안의 페이지는 보통 `../images/파일명` 형태로 두면 됩니다.
- 예전에 루트에 두었던 `backup/`·`_backup/` 복제 HTML은 정리되어 제거되었습니다. 필요 시 Git 히스토리에서 복구할 수 있습니다.
- 루트에 `index.html`이 있으면 기본 진입점으로 인식됩니다.

## 라이선스·저작권

사진·영상·텍스트는 개인 창작 및 안내 목적에 맞게 사용해 주세요. 외부 링크(블로그, Notion 등)는 각 서비스 정책을 따릅니다.

---

*Sky View — 위에서 본 풍경을, 화면 너머로 나눕니다.*
