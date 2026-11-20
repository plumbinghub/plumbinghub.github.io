# 배관설비 Hub (plumbing-hub)

무료 배관설비 계산기 — GitHub Pages용 정적 단일 페이지 사이트입니다.

**배포 주소:** https://plumbinghub.github.io/

## 사이트 소개

한국 설비 조건(KS 기준, 380V 3상 / 220V 단상, 60Hz)에 맞춘 한국어 배관 계산기 허브입니다. 순수 HTML5, CSS3, 바닐라 JavaScript만 사용했습니다. 프레임워크도, 빌드 단계도, 백엔드도 없습니다.

## 계산기 (모두 브라우저 안에서 계산)

1. **급수관경 계산기** — 필요 내경 D = √(4·Q/π·v), Hazen-Williams 마찰손실, KS 호칭경 추천 (15A–100A).
2. **배수관경 계산기** — 기구배수부하단위(FU)와 구배(1/50, 1/100, 1/200), 수평관·수직관 기준 관경표.
3. **수압·수두 계산기** — 가용 수두와 수압(kPa, kgf/cm², bar), 최저 수압 대비 여유 판정.
4. **펌프 양정·동력 계산기** — 전양정 H = 실양정 + 마찰손실, 축동력 P = ρ·g·Q·H/η, 추천 모터 정격, 월 전력량 추정치.
5. **온수기 용량 계산기** — 저장 탱크 용량, 필요 열량(kW, kcal/h, kWh), 온도 상승폭.

그 외 포함 내용: KS 급수관 관경별 유량표(15A–100A), 6편의 배관설비 실무 가이드, FAQ, 소개와 면책 조항.

## GitHub Pages 배포 방법

1. GitHub 사용자 **motorwindinghub** 아래에 공개 저장소 **plumbing-hub**를 만듭니다.
2. 이 폴더의 모든 파일(`index.html`, `guides/`, `README.md`, `favicon.svg`, `.nojekyll`)을 저장소 루트에 업로드합니다.
3. 저장소에서 **Settings → Pages → Build and deployment → Deploy from a branch → 브랜치 `main`, 폴더 `/ (root)` → Save**를 선택합니다.
4. 몇 분 안에 **https://plumbinghub.github.io/** 에서 사이트가 열립니다.

## 로컬 미리보기

```bash
python3 -m http.server 8000
# http://localhost:8000/ 에서 확인
```

## 면책 조항

모든 계산 결과는 참고용 추정치입니다. 실제 설계와 시공은 건축설비기준, KS 규격, 해당 지역 조례와 제조사의 설치 지침을 따라야 하며, 중요한 설비는 반드시 자격 있는 설비 기술자나 설계사무소의 검토를 받으세요.
