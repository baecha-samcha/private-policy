# AgentMesh privacy policy

AgentMesh 개인정보처리방침과 공개 서비스 소개 페이지. 빌드 도구·의존성·JavaScript 없이 동작합니다.

## Cloudflare Pages

Workers & Pages → Create application → Pages → Connect to Git에서 이 저장소를 선택합니다.

| 설정 | 값 |
| --- | --- |
| Production branch | `main` |
| Framework preset | None |
| Build command | `exit 0` |
| Build output directory | `public` |
| Root directory | 기본값 (저장소 루트) |

배포 완료 후 프로젝트 → Custom domains → Set up a custom domain에서
`private-policy.baecha.xyz`를 추가합니다. GitHub 저장소 생성만으로 배포나 DNS 설정이 완료되지는 않습니다.

공식 배포 안내: https://developers.cloudflare.com/pages/framework-guides/deploy-anything/

## Google Auth Platform 브랜딩

배포 후 로그아웃 상태에서 아래 두 주소가 HTTP 200으로 열리는지 먼저 확인합니다.

- 홈페이지 URL: `https://private-policy.baecha.xyz/about/`
- 개인정보처리방침 URL: `https://private-policy.baecha.xyz/`
- 앱 이름: `AgentMesh`
- 승인된 도메인: `baecha.xyz` (필요 시 소유권 확인)
- 사용자 지원 이메일: 운영자가 실제로 확인하는 Google 이메일

사이트의 Google API 데이터 처리 안내는 다음 공식 정책을 참고합니다.
https://developers.google.com/terms/api-services-user-data-policy

문서의 데이터 이용·외부 AI 전달·보관 안내는 운영 방식이 바뀌면 함께 갱신해야 합니다.
OAuth 앱 게시나 검증 완료를 보장하지 않습니다.

## 로컬 확인

```sh
python3 -m http.server 8080 --directory public
```

`http://localhost:8080/` 및 `/about/`에서 확인합니다.
운영자 문의는 OAuth 동의 화면의 지원 이메일 또는 이 저장소의 Issues를 사용합니다.
개인정보·토큰·문서 본문은 공개 이슈에 올리지 마세요.
