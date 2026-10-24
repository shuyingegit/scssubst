[English](README.md) · [中文](README.zh-CN.md) · [日本語](README.ja.md) · **한국어** · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)

<p align="center">
  <img src="docs/banner.svg" alt="ScsSubst" width="100%">
</p>

<h1 align="center">ScsSubst</h1>

<p align="center">
  <strong>폴더를 드라이브 문자로</strong><br>
  깊은 폴더에 드라이브 문자 — 복사 없이 로컬 디스크처럼.
</p>

<p align="center">
  <a href="https://subst.scsoi.com"><img src="https://img.shields.io/badge/Website-subst.scsoi.com-0F766E?style=flat-square" alt="Website"></a>
  <a href="https://github.com/shuyingegit/scssubst/releases/latest"><img src="https://img.shields.io/github/v/release/shuyingegit/scssubst?style=flat-square&label=Release" alt="Release"></a>
  <a href="https://subst.scsoi.com/#download"><img src="https://img.shields.io/badge/Windows-10%20%2F%2011-0078D4?style=flat-square&logo=windows&logoColor=white" alt="Windows"></a>
  <a href="mailto:support@scsoi.com"><img src="https://img.shields.io/badge/Support-support%40scsoi.com-6B7280?style=flat-square" alt="Support"></a>
</p>

<p align="center">
  <a href="https://subst.scsoi.com/#download"><strong>다운로드</strong></a> ·
  <a href="https://subst.scsoi.com/#pricing"><strong>가격</strong></a> ·
  <a href="https://github.com/shuyingegit/scssubst/releases"><strong>릴리스</strong></a> ·
  <a href="https://drive.scsoi.com"><strong>ScsDriver</strong></a>
</p>

---

## ScsSubst를 쓰는 이유

깊은 폴더에 드라이브 문자 — 복사 없이 로컬 디스크처럼.

파일을 쓰거나 지울 수 있는 도구를 쓸 때 범위를 넘어 지울까 걱정되나요? 못 나가는 작업 드라이브를.

<p align="center">
  <img src="docs/hero.png" alt="ScsSubst hero" width="920">
</p>

## 이런 용도로

- 자주 쓰는 폴더 → 드라이브
- 도구를 한 드라이브에 가두기
- 긴 프로젝트 경로 줄이기
- 작업 공간마다 드라이브

### 핵심: 더 안전한 샌드박스 작업 드라이브

**못 나가는 작업 드라이브를**

월권·오삭제가 걱정되면, 작업 폴더를 드라이브로 매핑하고 도구를 그 안에만 두세요.

1. 전용 작업 폴더 만들기
2. 드라이브로 매핑(예: Z:)
3. 도구 작업 공간을 Z:로

> 도구 작업 공간을 해당 드라이브로. 실용적 격리이며 OS 샌드박스는 아닙니다.

<p align="center">
  <img src="docs/sandbox-usecase.png" alt="ScsSubst sandbox use case" width="920">
</p>

## 핵심 기능

간단하고 안정적이며 번거롭지 않습니다.

- **원클릭 마운트** — 폴더와 드라이브 문자를 고른 뒤 연결하세요. 시작 시 자동 마운트도 가능합니다.
- **네이티브 경험** — 탐색기에서 일반 드라이브처럼 사용합니다. 경로가 짧아집니다.
- **자동 시작** — 앱을 열 때 저장한 매핑을 자동으로 다시 걸 수 있습니다.
- **경량 및 안정성** — Windows API만 사용. 서드파티 파일시스템 드라이버 없음.
- **여러 매핑** — 폴더 매핑을 여러 개 추가하고 각각 다른 드라이브 문자를 씁니다.
- **고급 옵션** — 관리자 앱 표시, 휴지통 등. 기본은 단순합니다.
- **설치 즉시 체험** — 기본 7일 체험. 이후 라이선스(월/년/평생)로 활성화.
- **샌드박스 작업 드라이브** — 쓰기 도구는 종종 범위를 넘어 파일을 지웁니다. 전용 폴더를 드라이브로 매핑하고 작업 공간을 그쪽으로 — 실수도 그 안에.


## 다운로드

최신 빌드: **[GitHub 릴리스](https://github.com/shuyingegit/scssubst/releases/latest)** · [웹사이트](https://subst.scsoi.com/#download)

| 패키지 | 용도 |
|--------|----------|
| **Portable (`.zip`)** | 압축 해제 후 실행(권장) |
| **Installer (`.exe`)** | 설치 프로그램 |

시스템 요구사항: Windows 10 / 11 (64비트)

## 가격

무료 체험은 7일부터. 친구를 초대하면 양쪽 모두 체험을 늘릴 수 있습니다.

모든 플랜(무료 체험 포함)에 기술 지원 포함. 사용 중 오류나 문제가 있으면 이메일로 알려주세요. 확인·수정하고 지속 개선하겠습니다.

## 관련 제품

WebDAV / 클라우드를 Windows 로컬 디스크로 마운트합니다.

→ **[ScsDrive](https://github.com/shuyingegit/scsdriver)** · [drive.scsoi.com](https://drive.scsoi.com)

## 자주 묻는 질문

**ScsSubst와 클라우드 마운트의 차이는?**  
ScsSubst는 PC에 이미 있는 폴더를 매핑합니다. 클라우드/WebDAV는 자매 제품 ScsDriver(drive.scsoi.com)를 사용하세요.

**체험판과 정식판의 차이점은 무엇인가요?**  
기능은 같습니다. 체험은 7일, 친구 초대 코드로 시작하면 14일이 됩니다. 친구가 내 코드로 체험을 시작하면 나도 +7일(제한 없음). 무기한 구매는 제외. 체험 후에는 라이선스가 필요합니다.

**ScsSubst로 안전 샌드박스 작업 드라이브를 만들려면?**  
전용 작업 폴더를 만들어 드라이브로 매핑하고, 도구 작업 공간을 그쪽으로 지정하세요. 실수로 지워도 그 드라이브 안에 남습니다. OS 수준 샌드박스는 아닙니다.

## 라이선스 및 약관

이용약관 · 개인정보 처리방침 · 환불 정책 — [https://subst.scsoi.com/terms](https://subst.scsoi.com/terms) · [https://subst.scsoi.com/privacy](https://subst.scsoi.com/privacy) · [https://subst.scsoi.com/refund](https://subst.scsoi.com/refund)

---

<p align="center">
  <a href="https://subst.scsoi.com/"><strong>웹사이트 열기 →</strong></a>
</p>
