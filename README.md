# ohmypower.ai

오마이파워 공개 사이트(정적). GitHub Pages로 배포합니다.

## 이 저장소에 넣지 않는 것
이 저장소는 **공개**로 둡니다. 아래는 별도의 비공개 저장소에 둡니다.
- 정은 시스템 프롬프트, 질문 설계, 직무 팩
- DB 스키마와 마이그레이션
- API 키와 비밀값(Fish Audio, Anthropic 등). 어떤 저장소에도 커밋하지 않습니다.

## 구조
- `index.html` 랜딩
- `404.html` 없는 주소
- `assets/style.css` 공통 스타일
- `CNAME` 커스텀 도메인 (GitHub Pages가 읽음, 지우지 말 것)
- `.nojekyll` Jekyll 처리 끄기

## 배포
`main` 브랜치 루트(/)에서 배포합니다. 푸시하면 1~2분 안에 반영됩니다.

## 다음 단계(오디오 연결)
Fish Audio와 Claude 호출은 브라우저에서 직접 하지 않습니다. 키가 노출되기 때문입니다.
서버 함수(Cloudflare Workers, Vercel 등)가 필요하며, 오디오 연결 단계에서 정합니다.
