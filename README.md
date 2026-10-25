# Did I Finish?

## 최신 관리 현황 — 2026-10-15

- 앱: Did I Finish? / com.ezekiel.didi / 앱 프로젝트: did-i
- 로컬 경로: C:\dev\EzekielDev\did-i-config
- 앱 단계: 프로덕션 액세스 승인 완료 / 2.0.1 프로덕션 Google 검토 중
- Play: 2.0.1 / code 3 · 프로덕션 제출, Google 검토 중. 이전 Alpha 2.0.0 / code 2
- 소스/native: 2.0.1 / 3 (세부 불일치·목표는 앱 README 참고)

### 공개 파일과 운영

privacy-policy.html

10/14 앱 작업 보고에서 공개 HTTPS 200·로컬 내용 일치 확인. db59b95 로컬 Git 확인; 이번 네트워크 재검증 없음. 공개 정적 파일용 저장소이며 앱 package/versionCode와 별도의 콘텐츠 형식을 유지한다. Secret·서명 파일·사용자 기록을 넣지 않는다.

### 현재 문제 / 다음 작업

프로덕션 액세스 승인·code 3 등록은 앱/Play 관리 항목. 새로 게시 완료된 정책을 미게시로 되돌리지 않는다.

### 개발 및 변경 이력 — 최신 날짜순

2026-10-15 사용자 제출/심사 상태와 앱 README 동기화. 공개 JSON·정책 내용 및 배포 상태는 새로 검증하지 않았다.

2026-10-14 정책 공개 일치 보고·db59b95. 2026-10-13 브랜드 문구 변경; 기존 URL 유지.

기존 JSON·정책 본문은 이번에 수정하지 않았다. 로컬 Git만으로 원격 게시 완료를 선언하지 않는다. [앱 최신 README](../did-i/README.md)에서 빌드·테스트·실기기 상태와 다음 작업을 함께 관리한다.

## 기존 운영 안내 및 작성 당시 기록

이하 게시 전/미구현 표현은 작성 당시 기록이다. 현재 상태는 상단을 우선한다.

Android 앱 Did I Finish?의 공개 개인정보처리방침 원본이다.

- 앱 package: `com.ezekiel.didi`
- 저장소명: `did-i-config` (앱 저장소: `did-i`)
- 정책 URL: https://ezekieldevstudio.github.io/did-i-config/privacy-policy.html
- 원본: `privacy-policy.html`
- 브랜드명은 12개 언어에서 모두 **Did I Finish?**로 유지한다.

## 2026-10-13 브랜드 변경

HTML의 제목·메타 설명·본문·푸터를 새 브랜드로 변경했다. URL과 데이터 처리 내용은 유지했다. 현재 v2의 로컬 기록·체크 시각·최근 이름, 1~3개 로컬 알림, 위젯별 테마/불투명도, 12개 언어, Android 시스템 백업 예외, AdMob/UMP 설명과 대조했다. 예전 한국어/영어 전용 추천 설명은 없다.

2026-10-14 확인: 공개 HTTPS URL은 200이며, Did I Finish? 브랜드가 반영된 로컬 privacy-policy.html과 내용이 일치한다. Calendar/history, Widget, Notifications, 로컬 저장 및 AdMob/UMP 설명은 현재 앱 구현과 일치한다. 정책 본문 추가 변경은 필요 없다.

Play Alpha 기존 등록은 2.0.0 / versionCode 2, 다음 제출 후보는 2.0.1 / versionCode 3이다. code 3 미사용 여부와 프로덕션 액세스 승인 여부는 사용자가 Play Console에서 확인한다.

## FAQ / 공지 정적 콘텐츠 — 로컬 준비, 미게시 (2026-10-25)

- 공통 HoopView 구조를 따르는 config.json: schemaVersion 1, content.faq/notices.{version,file}. 각 본문은 {version,items}. 초기 faq/notices 버전은 각각 1이며 서로 독립적이다.
- FAQ 행: id/order/enabled/question/answer/locales. 공지 행: id/enabled/publishedAt/title/body/locales. 기본 필드는 영어이며 locales는 en,ko,ja,es,pt,fr,de,it,zh-Hans,zh-Hant,id,vi의 필드별 번역이다. 공통 필드를 유지하고 다국어 필드만 확장했다. 누락/빈 번역 필드는 영어로 fallback한다. 알 수 없는 구조/필수값/잘못된 타입은 거부한다.
- faq.json: faq-001~008, 12개 언어의 질문/답변. notices.json: version 1, items:[] (공개 가능). 실제 배포 확인 근거가 없는 기능을 출시됐다고 안내하지 않는다.
- notices.draft.json: notice-001/002의 12개 언어 초안, enabled:false, publishedAt:null. 앱/config에서는 이 파일을 참조하지 않는다. 게시 파일이 아니며 공개 배포 대상에서도 제외한다. 출시 확인 후 공개할 항목만 실제 게시일 YYYY-MM-DD와 enabled:true로 notices.json에 옮긴다. 초안에 가짜 과거 게시일을 넣지 않았다.
- 준비 URL: https://ezekieldevstudio.github.io/did-i-config/config.json, faq.json, notices.json. 기존 privacy-policy.html 내용/URL은 그대로다. 이 작업에서 원격 게시하지 않았다.
- 수정할 때 해당 본문 version과 config.content의 해당 version을 함께 올린다. 본문을 먼저 게시하고 config를 마지막에 게시한다. FAQ 변경에 notices 버전을 올리지 않는다. 앱은 본문 버전 일치까지 검증하며 불일치·다운로드·캐시 저장 실패 시 마지막 정상 콘텐츠를 유지한다.
- 앱 검증: did-i에서 node scripts/check-help.cjs. 8×12 FAQ와 2×12 공지 초안, 캐시/실패 조합 집중 검증. 로컬 에뮬레이터 공지 상세 검증은 테스트 응답을 이용했으며 공개 JSON에는 추가하지 않았다.
- 게시 전 12개 언어 내용과 실제 배포 버전, 게시일을 확인한다. commit/push/GitHub Pages/Play 등록은 별도 승인 후 진행한다.
