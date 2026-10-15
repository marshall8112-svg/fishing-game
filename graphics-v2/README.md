# 바다 찌낚시 그래픽 V2.2 — 포토리얼 조과 이미지

## 로컬 실행

저장소 전체를 다운로드하거나 git pull한 뒤 `graphics-v2/fishing-demo.html`을 Chrome/Edge에서 엽니다. **HTML 파일과 ait-project 폴더를 함께 보관**하세요. 새 PNG 파일 2개가 필요합니다.

```powershell
Start-Process .\fishing-demo.html
```

오른쪽 **잡은 물고기 미리보기**를 반복해서 누르면 26종을 확인합니다. 미리보기는 실제 조과나 보상에 기록되지 않습니다.

## 변경

잡은 물고기 결과 화면은 사진에 가까운 AI 생성 PNG로 표시합니다. 미역치·독가시치·황어·성대는 별도 이미지 시트를 사용합니다. 비늘, 젖은 피부, 실제 같은 지느러미와 눈 표현을 사용하며 배경은 투명합니다.

이미지는 게임 연출용 AI 생성물이며 실제 촬영 사진이나 정확한 어종 식별 자료가 아닙니다. 이미지가 로드되지 않으면 V2.1 절차적 그림으로 대체합니다. 도감·조과 목록의 작은 아이콘 및 수중 3D 모델은 V2.1을 유지합니다.

파일: `ait-project/public/fish-photos/coastal-atlas.png`, `special-atlas.png`. 이미지 생성 사양은 `ASSET_SPECS.md` 참조.

검증: 26종 이미지 매핑과 Canvas 실제 렌더링 통과, 6종 화면 시각 검토, JavaScript 문법 및 기존 모델 검사 통과. 전체 브라우저 조작·성능과 토스 SDK 빌드는 미검증입니다.
