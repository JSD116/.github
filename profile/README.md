# JSD116

Duofund 프로젝트의 제품 기준, 웹앱, 백엔드 API, 운영 문서를 함께 관리하는 GitHub Organization입니다.

<p align="center">
  <img src="assets/mascot/duofund-mascot.png" alt="Duofund mascot" width="260" />
</p>

## Duofund

Duofund는 커플 / 공유 가계부를 위한 서비스입니다. 공동 계좌와 개인 계좌를 분리하고, 월 예산, 거래 기록, 자산 추이, 미션 기반 습관 관리를 한 흐름에서 다룹니다.

## Repositories

- [duofund-spec](https://github.com/JSD116/duofund-spec): 제품 기준, 도메인 규칙, 운영 정책, 로드맵 문서
- [duofund-app](https://github.com/JSD116/duofund-app): Next.js 15 / React 19 기반 웹앱
- [duofund-server](https://github.com/JSD116/duofund-server): Kotlin / Spring Boot 기반 REST API와 OpenAPI 문서

## Current Product Surface

- Web App: 홈, 기록, 자산, 미션, 설정
- Backend API: 인증 / 세션, 프로필 이미지, 그룹, 계좌, 거래, 예산, 자산, 예산 스냅샷, 통계
- Mission Board: 현재 웹앱 로컬 저장 기반, 서버 동기화는 후속 범위
- API Docs: `duofund-server/docs/api/openapi-v1.yaml` 기준

## Branding

- app mascot source: `duofund-app/public/pwa-maskable-512.png`
- spec/profile copy: `duofund-spec/assets/mascot/duofund-mascot.png`
- organization profile copy: `.github/profile/assets/mascot/duofund-mascot.png`

세 파일은 같은 PNG를 유지합니다.

## Deployment

- Frontend: Cloudflare Pages
- Backend: self-hosted Compose primary, Railway fallback policy maintained
- CI/CD: GitHub Actions

## Team Workflow

- 제품 / 도메인 기준은 `duofund-spec`에서 먼저 정리합니다.
- 구현 변경은 `duofund-app` / `duofund-server`에서 PR 기반으로 반영합니다.
- API 계약은 `duofund-server` OpenAPI 소스와 번들 스펙을 기준으로 검증합니다.
- 운영 정책과 runbook은 `duofund-spec/policy`와 `duofund-spec/roadmap`에서 관리합니다.
