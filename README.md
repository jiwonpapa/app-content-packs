# App content packs

여러 앱의 공개 콘텐츠를 GitHub Releases로 전달하는 자료 전용 저장소입니다. 앱 소스 코드는 포함하지 않습니다.

## 현재 상태

2026-10-20: HangulPlay dev 채널에 [새 선 놀이 v1](https://github.com/jiwonpapa/app-content-packs/releases/tag/hangulplay-dev-2026.10.20.1)을 배포했습니다. 0.5.0-dev 앱의 보호자 설정에서 서명을 검증하고 받을 수 있습니다. 원본 기하 선 3종·활동 6회의 개발용 자료이며 교육 검수 전입니다. production은 `not_ready`를 유지합니다. 초기 bootstrap 릴리스는 앱 설치 대상이 아닙니다.

## 앱별 배포

| 앱 | 채널 | 목록 진입점 | 릴리스 태그 접두어 |
|---|---|---|---|
| HangulPlay | production | [production head](heads/hangulplay/production.json) | `hangulplay-production-` |
| HangulPlay | dev | [dev head](heads/hangulplay/dev.json) | `hangulplay-dev-` |

앱은 자신에게 고정된 head만 조회합니다. 저장소 전체의 `releases/latest`를 앱별 최신 자료로 사용하지 않습니다. 다른 앱을 추가할 때는 별도의 appId·head·릴리스 접두어·신뢰 범위를 등록합니다. 한 릴리스에 여러 앱의 팩을 섞지 않습니다.

작은 JSON head는 Git에서 관리하고 큰 학습팩은 Release asset으로 제공합니다. [배포 규약](DISTRIBUTION.md)을 따릅니다.

## 권리와 개인정보

공개 자료는 누구나 내려받을 수 있습니다. 공개 상태 자체가 재사용·재배포·상업 이용 허가를 뜻하지 않습니다. 각 팩에 출처·사용권·검수 정보를 명시합니다. 이 저장소에 비밀키·인증 토큰·아동 개인정보·원본 필기 기록을 넣지 않습니다. 승인되지 않은 학습자료·음성·이미지도 발행하지 않습니다.
