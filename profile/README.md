# JSD116

Duofund 프로젝트의 제품/앱/서버를 함께 운영하는 GitHub Organization입니다.

<p align="center">
  <img src="assets/mascot/duofund-mascot.png" alt="Duofund mascot" width="320" />
</p>

## Repositories
- [duofund-spec](https://github.com/JSD116/duofund-spec): 비즈니스 기획, 도메인 스펙, 운영 정책 문서
- [duofund-app](https://github.com/JSD116/duofund-app): Next.js 기반 웹앱 프론트엔드
- [duofund-server](https://github.com/JSD116/duofund-server): Spring Boot 기반 백엔드 API

## Deployment
- Frontend: Cloudflare Pages (production)
- Backend: Railway (duofund-api)
- CI/CD: GitHub Actions (`main` merge 시 자동 배포)

## Team Workflow
- 스펙 변경은 `duofund-spec`에서 먼저 합의
- 구현 변경은 `duofund-app`/`duofund-server`에서 PR 기반 반영
- 운영 정책은 `docs/policy`에서 관리
