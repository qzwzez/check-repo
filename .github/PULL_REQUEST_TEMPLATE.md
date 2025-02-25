## What

- 로그인 API 요청 로직을 추가했습니다.
- JWT 토큰을 저장하고, 인증이 필요한 요청에 헤더를 추가하도록 구현했습니다.

## Why

- 기존에는 로그인 기능이 없어서 사용자가 접근할 수 없었습니다.

## How

- `POST /api/login` 요청을 통해 서버에서 JWT를 받아 저장하도록 구현
- `axios` 인터셉터를 이용해 인증이 필요한 요청에 자동으로 `Authorization` 헤더 추가
- `zustand`를 이용해 로그인 상태 관리

## Demo

![로그인 성공](https://example.com/login_success.png)

## Checklist

- [x] 기능 구현 완료
- [x] API 테스트 완료
- [ ] 에러 처리 추가
