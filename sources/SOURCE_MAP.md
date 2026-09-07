# 원문 추적표

이 저장소는 `appback/appback-platform` 저장소의 `appback-hub/docs`를 서비스 관점으로
재구성한다. 아래 표는 각 문서의 주요 근거다. 원문의 API 예시, DB 구조와 배포 절차는
그대로 복제하지 않고 서비스 의미만 추렸다.

기준 확인일: 2026-09-07

| 이 저장소 문서 | 주요 원문 |
| --- | --- |
| `README.md` | `docs/HANDOVER.md`, `docs/api/internal-response-contract.md`, `docs/first-run-tutorial-page-scenario.ko.md` |
| `00-feature-status.md` | `docs/README.md`, 각 기능 문서의 Scope·상태 문구 |
| `01-service-overview.md` | `docs/HANDOVER.md`, `docs/first-run-tutorial-page-scenario.ko.md`, `docs/offerwall-launcher-v4-contract.md` |
| `02-user-journey.md` | `docs/first-run-tutorial-page-scenario.ko.md`, `docs/pending-rewards-api.md`, `docs/app-asset-history-webview-guide.md`, `docs/support-ticket-admin-guide.md` |
| `03-star-and-rewards.md` | `docs/pending-rewards-api.md`, `docs/app-referral-streak-guide.md`, `docs/HANDOVER.md` |
| `04-quests-and-offerwalls.md` | `docs/offerwall-launcher-v4-contract.md`, `docs/offerwall-provider-onboarding.md`, `docs/support-ticket-admin-guide.md`, provider별 README |
| `05-gifticon-shop.md` | `docs/admin-gifticon-product-management.md`, `docs/gifticon-timesale.md`, `docs/gifticon-identity-account-binding.md`, `docs/support-ticket-admin-guide.md` |
| `06-content-and-messaging.md` | `docs/promotions-api.md`, `docs/promotion-v2-contract.md`, `docs/home-promotions.md`, `docs/app-announcements.md`, `docs/in-app-messages-status-plan.md` |
| `07-support-and-safety.md` | `docs/support-ticket-admin-guide.md`, `docs/support-inquiry-ai-response-guide.md`, `docs/user-event-policy-contract.md` |
| `08-operations-and-ownership.md` | `docs/HANDOVER.md`, `docs/api/internal-response-contract.md`, `docs/offerwall-launcher-v4-contract.md`, `docs/admin-gifticon-product-management.md` |
| `09-glossary.md` | 위 문서 전체의 사용자·운영 용어 |

## 상태 판정 시 주의할 원문

- 파일명에 `plan`, `design`, `proposal`, `handoff`가 있으면 구현·운영 여부를 별도로 확인한다.
- `home-promotions.md`는 구버전 호환 계약이고 신규 프로모션의 단일 기준이 아니다.
- `in-app-messages-status-plan.md`와 관련 앱 가이드는 상세하지만 운영 활성 여부의 증거는 아니다.
- `offerwall-reward-buff-system-plan.md`는 계획이며 현재 제공 기능으로 소개하지 않는다.
- 친구초대 14일 이벤트는 기능 존재와 현재 활성화를 구분한다.
- 원문의 날짜별 운영 증거는 장기 서비스 설명의 원본으로 사용하지 않는다.

## 갱신 규칙

1. 먼저 원문에서 현재 계약인지 계획인지 확인한다.
2. 사용자 경험, 운영 책임 또는 정책 의미가 달라질 때만 이 저장소를 갱신한다.
3. API 필드명만 바뀌고 사용자 경험이 같다면 원문만 갱신할 수 있다.
4. 사용자에게 노출되는 이름, 재화, 보상 조건, 구매 상태, 문의 정책이 바뀌면 반드시 반영한다.
5. 근거가 충돌하면 추측하지 않고 기능 상태를 `확인 필요`로 낮춘다.
