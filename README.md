# app-factory-assets

app-factory 앱들이 **실행 중에** 받아 쓰는 공개 이미지 에셋입니다. 앱 업데이트 없이 그림을 늘리기 위한 저장소입니다.

- 게시: GitHub Pages — `https://johyunchol.github.io/app-factory-assets/<slug>/ledger.json`
- 구조: 앱별 폴더 `<slug>/ledger.json` + `<slug>/bg/*.webp`
- 원장 한 줄 = 그림 한 장: `file`·`season`·`prompt`·`tool`·`model`·`created`·`terms_version` (+선택 `calm`·`snow`), `sha256`·`bytes`
- 앱은 원장을 받은 뒤 그림마다 `sha256`·형식·크기를 검증하고 통과한 것만 씁니다.

## greeting_card (다정인사)

카드 배경 — 4:5 세로 1080×1350 WebP, 장당 200KB 이하. 아래 40% 는 글자 띠 자리라 단순하게 비워 둡니다.
제작: Codex 이미지 생성(Paseo, `gpt-6.1-sol`) — 원장의 `terms_version` 참고. 규칙·절차는 app-factory 저장소 CLAUDE.md '원격 이미지 에셋' 섹션이 기준입니다.
