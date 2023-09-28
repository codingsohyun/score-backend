# 스코어 백엔드 개발

## ==== 230918 ====
### 로그인/회원가입
 - [ ] 클라이언트에서 인증이 완료된 후 받은 id 값 받기 -> db에 해당 유저 id 값과 일치하는 유저 정보가 있는지 확인
   - [ ] 존재하지 않는다면 (회원가입 필요한 경우) 새로운 회원 엔티티 생성 
     - [ ] 새로운 jwt 토큰 발급 후 서비스 메인 화면으로 접속
   - [ ] 존재한다면 (기존 회원인 경우) jwt 토큰 만료 여부 검증
     - [ ] 만료되지 않았다면 서비스 메인 화면으로 접속
     - [ ] 만료되었다면 refresh token을 통해 토큰 갱신
   - [ ] 기타 인증 오류 관련 예외 처리

### 패키지 구조 리팩토링

