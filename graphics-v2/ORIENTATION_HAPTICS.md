# 가로 화면 · 감기 진동 수정

- 회전 안내가 게임을 차단하지 않도록 제거했습니다.
- 앱인토스 Screen.setOrientation으로 가로 화면을 요청하고, 실패하거나 WebView가 세로로 남으면 게임 영역을 가로로 회전합니다.
- 세로 WebView의 ↻ 버튼으로 회전 방향을 반대로 바꿀 수 있습니다.
- 물고기와 힘겨루기하며 감는 동안 Device.triggerHaptic을 간격을 두고 호출합니다. 줄 장력이 높으면 진동을 강화하며, 감기를 멈추거나 앱을 떠나면 중단합니다.
- HUD의 진동 켬/끔 버튼으로 설정할 수 있습니다. 지원되지 않는 환경에서도 게임은 계속 실행됩니다.

검증: Vite 및 ait build 성공, JavaScript 문법 검사, 회전 상태/진동 간격 모의 테스트 통과. 실제 토스 iOS/Android 기기 확인은 별도로 필요합니다.

재빌드: `npm install`, `npm run build`, `npx ait build` (빌드 환경 SDK 3.8.0).
