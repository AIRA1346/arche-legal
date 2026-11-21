# ARCHE (아르케) 개인정보처리방침 · Privacy Policy

- **시행일 / Effective Date:** 2026-11-21 (`v1.0`)
- **운영자 / Operator:** Runic Atelier (ARCHE 창립자 / Founder)
- **대상 앱 / Application:** ARCHE (Steam AppID `5560360`) 및 연동 웹·API 서비스
- **문의 및 요청 / Contact:** `runicatelier@gmail.com`

---

## [한국어] 개인정보처리방침

### 1. 수집하는 정보와 수집하지 않는 정보
ARCHE는 무료 공동 세계관 읽기·탐구·제작 소프트웨어로서 서비스 운영에 꼭 필요한 최소 정보만 처리합니다.

1. **인증 및 계정 식별 정보 (공동 작성 서버 로그인 시)**
   - **수집 항목:** Steam OpenID 또는 Steam 인증 티켓으로 검증된 **SteamID64**, ARCHE 내부 식별자(`userId`), 계정 활성/중단 상태 및 참여 권한 상태.
   - **수집하지 않는 항목:** ARCHE는 사용자의 **Steam 비밀번호, Steam Guard 코드, 결제·카드 정보, 실명·주민등록번호·전화번호**를 요구하거나 저장하지 않습니다.
2. **사용자가 명시적으로 제출한 공동 창작 자료**
   - 정식 제안(원문·설명), 토론 의견, 번역 연결, 참고용 이미지(PNG/JPEG), 외부 참고 URL 및 첨부 메타데이터(출처, 작성 시각, 수정·정정 이력).
   - **기기 로컬 보관 구분:** 사용자가 명시적으로 제출하지 않은 **개인 초안, 개인 질문, 읽던 위치, 북마크, UI 언어·패널 설정(`ui-preferences.json`)**은 기본적으로 사용자의 PC(`%LOCALAPPDATA%`)에만 저장되며 서버로 자동 전송되지 않습니다.
3. **최소 보안·운영 기록**
   - 악용 방지, 오류 진단, 접근 권한 검증을 위한 요청 시각, HTTP 상태·오류 코드, 속도 제한 및 세션 검증 메타데이터.
   - ARCHE는 제3자 광고 추적기(Ad Tracker)나 맞춤형 광고 프로파일링을 사용하지 않으며, 개인정보를 제3자에게 판매하지 않습니다.

### 2. 정보의 이용 목적
- Steam 신원 확인 및 참여자 권한·접근 회수 검증
- 공동 세계관의 제안·토론·검토·승인·채택·정정·번역 이력 유지
- 저작권·유해물 신고 대응, 서비스 악용 차단 및 장애 복구(암호화 백업)

### 3. 보관 기간 및 암호화 백업
- **계정·신원 정보:** 계정 활성 기간 동안 보관합니다.
- **재해복구(DR) 외부 백업:** 데이터 유실 방지를 위해 외부 오브젝트 스토리지(Cloudflare R2 등)에 **AES-256-GCM으로 암호화**된 스냅샷을 **최대 30일간 순환 보관** 후 자동 삭제합니다. 재해 복원 시 사후에 회수된 계정 상태(`postSnapshotRevocations`)를 반영해 중단 계정이 부활하지 않도록 보호합니다.
- **보안·접속 로그:** 장애 분석 및 보안 대응 목적 달성 후 최대 90일 이내 파기합니다.

### 4. 계정 탈퇴, 삭제 요청 및 저자 이름 익명화
사용자는 언제든지 `runicatelier@gmail.com`으로 계정 중단·삭제 또는 저자 표기 익명화를 요청할 수 있습니다.
1. **즉시 삭제 대상:** 미제출 개인 자료(로컬 기기 파일은 사용자가 직접 삭제 가능), SteamID 연결 정보 및 활성 로그인 세션.
2. **공동 세계관 정본·공유 기록의 보존과 익명화:** 이미 공동 토론에 제출되었거나 ARCHE 세계관 정본에 채택·통합된 글·설정·의견은 다른 참여자의 설정과 연결된 공유 기록이므로 [이용약관 및 기여자 약관](TERMS-AND-CONTRIBUTION-LICENSE.md)에 따라 삭제되지 않고 보존됩니다. 다만 사용자가 요청할 경우 **작성자 표시 이름(크레딧)을 익명 표기(예: `Anonymous Contributor`)로 변경**해 드립니다.
3. **암호화 백업 반영:** 삭제·익명화 처리 후 기존 30일 암호화 DR 스냅샷은 순환 주기가 지나면 자동 만료됩니다.

### 5. 제3자 서비스 및 국외 이전 고지
ARCHE는 로그인·배포·보관 인프라로 아래 외부 서비스를 사용할 수 있으며, 각 서비스의 처리는 해당 사업자의 개인정보처리방침을 따릅니다.
- **Valve Corporation (Steam):** 앱 배포(SteamPipe), Steam OpenID / Steam 인증 티켓 신원 검증
- **Cloudflare, Inc.:** DNS, 보안 터널/프록시, 정적 판본 CDN 및 AES-256-GCM 암호화 백업 보관(R2)
- **운영 서버 호스팅(해당 시):** 초기 운영 환경(운영자 호스트 또는 클라우드 리전 VPS)

위 서비스 이용 과정에서 데이터가 대한민국 외의 글로벌 서버(미국·유럽·아시아 리전 등)에 전송·보관될 수 있으며, 모든 전송은 HTTPS(TLS)로, 외부 백업은 AES-256-GCM으로 암호화합니다.

### 6. 아동·청소년 보호
ARCHE는 Steam 플랫폼을 통해 제공되며, 각 지역 법령 및 Steam 이용약관이 정한 최소 이용 연령 미만의 아동으로부터 의도적으로 개인정보를 수집하지 않습니다.

### 7. 정책 변경 및 문의
본 방침이 변경되는 경우 변경 내용과 시행일을 GitHub 공개 정책 페이지 및 앱 안내에 고지합니다. 개인정보 열람·정정·계정 해지·저자 익명화 요청은 **`runicatelier@gmail.com`**으로 연락해 주세요.

---

## [English] Privacy Policy

### 1. Information We Collect (and Do Not Collect)
ARCHE is a free collaborative worldbuilding and reading software application. We minimize data collection to what is strictly necessary to run the service:

1. **Authentication & Account Identity (when signing in to the collaborative server)**
   - **Collected:** Your verified **SteamID64** (via Steam OpenID or Steam Auth Ticket), an internal ARCHE `userId`, and your participation/revocation status.
   - **Never Collected:** ARCHE never asks for or stores your **Steam password, Steam Guard codes, payment/card details, real name, government ID, or phone number**.
2. **Collaborative Content You Explicitly Submit**
   - Proposals, explanations, discussion comments, translation links, reference images (PNG/JPEG), external reference URLs, and revision/attribution metadata.
   - **Local-First Boundary:** Unsubmitted **private drafts, personal questions, reading positions, bookmarks, and UI preferences (`ui-preferences.json`)** stay locally on your own computer (`%LOCALAPPDATA%`) and are not automatically uploaded to our server.
3. **Minimal Security & Operational Logs**
   - Timestamps, HTTP status/error codes, rate-limiting signals, and session validation metadata strictly for security, abuse prevention, and debugging.
   - ARCHE uses **no third-party advertising trackers** and **never sells personal data**.

### 2. How We Use Information
- Verify Steam identity and enforce participation permissions or access revocations.
- Maintain transparent authorship, discussion, review, adoption, correction, and translation history for the shared ARCHE world.
- Investigate copyright/abuse reports, prevent spam or tampering, and perform encrypted disaster recovery backups.

### 3. Data Retention & Encrypted Backups
- **Identity Records:** Retained while your participation account remains active.
- **Encrypted Off-Host DR Backups:** Encrypted with **AES-256-GCM** and stored in off-host object storage (e.g., Cloudflare R2) on a **30-day rolling retention cycle**, after which older snapshots are deleted. Cold disaster restores enforce post-snapshot revocations so suspended accounts cannot be reinstated.
- **Security Logs:** Deleted within 90 days unless required to investigate an active security incident.

### 4. Account Deletion vs. Shared World Preservation & Anonymization
You may email `runicatelier@gmail.com` at any time to deactivate your account, delete private account linkage, or request author credit anonymization:
1. **Deleted Upon Request:** Your SteamID account link, active session, and any unsubmitted private account data (local files on your PC can be deleted directly by you at any time).
2. **Preserved Shared/Canonical Contributions (Anonymization Available):** Once submitted to shared discussion or integrated into the ARCHE world, lore entries, proposals, and comments remain part of the shared world record under our [Terms & Contribution License](TERMS-AND-CONTRIBUTION-LICENSE.md) and are not deleted. However, upon request, we will **anonymize your public display name/credit** (e.g., replacing it with `Anonymous Contributor`).
3. **Backup Expiry:** Encrypted DR snapshots age out automatically on the 30-day rolling cycle.

### 5. Third-Party Infrastructure & International Transfers
ARCHE relies on third-party infrastructure providers including **Valve Corporation (Steam)** (distribution and authentication) and **Cloudflare, Inc.** (DNS, encrypted tunnel/CDN, and encrypted R2 storage). Data may be processed across global data centers protected by HTTPS/TLS in transit and AES-256-GCM encryption for off-host backups.

### 6. Age Eligibility
ARCHE is distributed via Steam and is not directed to children under the minimum legal age required by Steam and applicable local law.

### 7. Changes & Contact
Material updates to this Privacy Policy will be published on this public policy repository with an updated effective date. For any privacy inquiry, account deactivation, or credit anonymization request, contact **`runicatelier@gmail.com`**.
