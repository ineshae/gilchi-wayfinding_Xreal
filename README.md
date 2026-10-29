# 길치를 위한 길찾기 서비스

지도를 읽지 않아도 되는 길찾기 프로토타입이에요. 가야 할 쪽에서 음악이 들리고, 음악 구슬과 바닥의 빛 물결이 3D로 길을 보여 줘요.

**바로 열기:** https://ineshae.github.io/gilchi-wayfinding_Xreal/

| 페이지 | 내용 |
| --- | --- |
| [`index.html`](https://ineshae.github.io/gilchi-wayfinding_Xreal/) | 메인 서비스: 지하철역 · 버스 · 골목 길찾기, 2D 지도와 AR 1인칭 화면, 구현 체크리스트 |
| [`vr.html`](https://ineshae.github.io/gilchi-wayfinding_Xreal/vr.html) | VR 버전: Quest 같은 헤드셋 브라우저에서 WebXR로 장면 안에 들어가 걷기. 헤드셋이 없으면 드래그 · 기울이기 · 카드보드 분할 화면으로 볼 수 있어요 |
| [`ar.html`](https://ineshae.github.io/gilchi-wayfinding_Xreal/ar.html) | AR 버전: Android 크롬(ARCore)에서 실제 바닥에 길 안내 띄우기. 아이폰 등은 카메라 화면 + 기울기 센서로 볼 수 있어요 |
| [`game.html`](https://ineshae.github.io/gilchi-wayfinding_Xreal/game.html) | 리듬 길찾기 게임: 서울역 · 홍대입구 · 지옥에서 노래에 맞춰 튀어나오는 것들을 쳐내며 목적지까지 가기. 키보드 · 터치 · VR 컨트롤러 |

## 리듬 길찾기 게임 조작

길은 직접 찾아가요. 걷는 동안 노래 박자에 맞춰 양옆에서 튀어나오는 것들을 쳐내요.

- 걷기: `W` `A` `S` `D` (또는 `↑` `↓`), `Shift` 뛰기. 휴대폰은 왼쪽 아래 조이스틱, VR은 왼손 스틱
- 왼쪽 노트: `←` 또는 `J` · 오른쪽 노트: `→` 또는 `K` · 노란 양쪽 노트: `Space`
- 지도: 왼쪽 아래 (파란 선이 가야 할 길, 노란 마름모가 목적지), `M`으로 크게 보기
- 반대로 가면 노래가 먹먹해지고 빛 물결이 주황색으로 바뀌어요
- `Q`: 자동 걷기 (리듬만 하고 싶을 때) · `Esc`: 일시정지

## 참고

- 음악(`music/`)은 blueblackines가 직접 만든 곡이에요.
- WebXR VR은 Quest 브라우저 같은 헤드셋 브라우저에서, WebXR AR은 ARCore를 지원하는 Android 크롬에서 동작해요. 아이폰 사파리는 WebXR을 지원하지 않아서 화면 대체 모드로 열려요.
- 카메라 · 기울기 센서 · WebXR은 HTTPS에서만 동작해서 GitHub Pages 주소로 열어야 해요.
- 체크리스트 수정 내용은 GitHub 페이지에서는 그 브라우저에만 저장돼요.
- `길치 서비스 최종.html`은 처음 올린 단일 파일 버전(음악 내장)이에요.
