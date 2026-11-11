# ai-native

AI 도구를 활용한 개발을 위한 공통 지침과 GitHub 설정 템플릿입니다.
특정 AI 도구나 언어·프레임워크에 종속되지 않습니다.

## 구성

- [AGENTS.md](AGENTS.md): AI 개발 도구가 따를 공통 작업 지침
- [main.json](.github/rulesets/main.json) / [dev.json](.github/rulesets/dev.json): 브랜치 룰셋
- [PR 템플릿](.github/PULL_REQUEST_TEMPLATE.md): 변경 내용과 검증 결과를 정리하는 기본 양식
- [Prettier 설정](templates/prettier/prettier.config.mjs): 프로젝트에서 선택해 사용하는 포맷 설정

## 사용 방법

1. **Use this template**으로 새 저장소를 생성합니다.
2. README를 프로젝트 소개와 사용법으로 교체합니다.
3. AGENTS.md에 프로젝트별 지침을 보완합니다.
4. 브랜치 룰셋을 가져와 적용하고, PR 템플릿을 필요에 맞게 조정합니다.

## Prettier 설정 사용

기존 포매터가 없고 Prettier를 선택한 프로젝트에서 사용합니다.

1. `templates/prettier/prettier.config.mjs`를 프로젝트 루트로 복사합니다.
2. 프로젝트의 패키지 매니저로 Prettier를 개발 의존성에 추가합니다.
3. 포맷 적용·검사 스크립트를 추가하고, 변경한 파일에 실행합니다.

설정 파일만으로 자동 실행되지는 않습니다. 템플릿 경로에서는 자동 탐색되지 않으며,
기존 포매터가 있다면 해당 설정과 실행 방식을 유지합니다.
