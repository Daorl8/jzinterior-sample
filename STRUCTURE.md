# STRUCTURE · jzinterior-sample (v0.1.0 · 스플릿 포트폴리오 · 스톤 바탕 + 차콜 · 모서리 2px · 배포 예정 jzinterior-sample.lgt3232.workers.dev)

```
jzinterior-sample/
├─ index.html                 단일 파일 (CSS · JS 인라인)
├─ wrangler.toml              name = jzinterior-sample
├─ .assetsignore              img/ · _old/ · 문서 · index_*.html · _deploy 배포 제외
├─ jz-cormorant.woff2         영문 워드마크 · 섹션 제목 (Cormorant Garamond 400–700, 영문만)
├─ jz-pretendard.woff2        본문 · 한글 (Pretendard 300–700, 페이지 글자 전부)
├─ jz-mark.svg                JZ 모노그램 (인스타 #41 벡터화)
├─ jz-hero.webp               히어로 (#46, 3:2)
├─ jz-f1 ~ jz-f6.webp         갤러리 전체 폭 3:2
├─ jz-p1a/b ~ jz-p6a/b.webp   갤러리 두 장 나란히 4:5
├─ favicon.png · og-jz.jpg
├─ img/                       다올 제공 원본 81장 + _원문.md (배포 제외 · 레포에 올리지 말 것)
└─ CHANGELOG.md / STRUCTURE.md
```

## 구조
- 1080 이상: `.wrapx` 2열 = `aside.side`(sticky 100vh · 마크 · 소개 · 메뉴 · 버튼 3 · 예약제 · 주소) + `main`(`#portfolio` 갤러리 → `#about` → `#contact` → 푸터).
- 1080 미만: `.top` 헤더(마크 · 상담신청서) + `.snav`(3개) → `aside`(히어로 사진 + 소개 + 버튼) → `main`(갤러리는 `.g-hero` 숨김) → 하단 바 `.quick`(상담신청서 · 전화).

## 버튼 · 링크
- 상담신청서 `https://form.naver.com/response/vbP0J4fB3rmPPbCHVwTF_g`(메인): 모바일 헤더 · 패널 · 문의 · 하단 바
- 전화 `tel:01033309634`: 패널 · 문의 · 푸터 · 하단 바
- 인스타 `https://www.instagram.com/jzinterior_director/`: 패널 · 문의 · 푸터
- 네이버 지도 `map.naver.com/p/entry/place/1184992824` · 블로그 · 네이버 플레이스(푸터)

## 모션 (강제 재생 · 다올 방침)
- 패널 `.intro` 등장 · 섹션 `.reveal`(setInterval) · 앵커 rAF 스크롤(R-25). reduced-motion 분기 없음.

## 폰트 재생성
문구 바꾸면 빠진 글자 검사(LESSONS §26). 한글은 Pretendard만, Cormorant는 영문 · 숫자만.
