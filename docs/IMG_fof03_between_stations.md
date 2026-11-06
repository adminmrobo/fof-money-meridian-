# 03번 「금융기관끼리 — 정거장 사이의 연결」 이미지 제작 명세서

> **그림 반영 (2026-11-07):** 표지·목차 카드·공유 미리보기·본문 컷·아웃트로 그림을 받아 저장소 루트에 WebP/JPG로 올리고 페이지에 넣었다. 히어로 무대 컷(`sc_fof03_hero`)은 선택 항목이라 아직 숨김 상태다.

| 항목 | 내용 |
|---|---|
| 페이지 | 03_fof_between_stations.html |
| 모드 / 주 앵커 | 교과서 모드 / D 생활·현장: 연구실 축소 모형 환승역과 선로(금융기관 간 연결), 보조 C 장부 |
| 시즌 | 기본 |
| 대결 | 장난감 금융망에 충격 4가 오면 고리형이 두 무리보다 덜 무너지는가 → 결과 F (초파리 승: 고리형 4곳, 두 무리 3곳, 완전 연결 1곳) |
| 새로 그릴 그림 | P1 2장 · P2 2장 · P3 2장 |
| 재사용 | 표정 18장 (캐릭터 팩 96px, 페이지에 base64로 들어 있음) |
| 그림이 없을 때 | 표지는 캔버스 대체 표지(역 다섯 + 선로 + 캐릭터 넷), 나머지 칸은 숨김 상태라 페이지는 완성 상태 |

## 1. 그림체와 고정 외형
- 스타일: SKILL 18-3 (16비트 RPG 픽셀아트, 굵은 외곽선, 2~3단계 명암)
- 캐릭터 고정 외형: 캐릭터 팩 18-4 그대로
- 이 페이지 장소: 밤의 연구실 탁자 위 환승역 축소 모형 다섯 곳(한국은행 금색·예금취급기관 하늘·투자펀드 자홍·보험연금 보라·기타금융기관 청록)과 빛나는 선로
- 장소 영어 묘사: *a night laboratory with a tabletop miniature of five round transit stations connected by glowing rails*

## 2. 필요한 그림 전체

| # | 키 | 판 | 크기 | 상태 | 우선 | 들어가는 곳 | 대신 쓰는 그림 |
|---|---|---|---|---|---|---|---|
| 0 | cover_fof03 | L | 1920×1080 | 새로 (COVER_fof03_between_stations.md) | P1 | 맨 위 글 표지 | 캔버스 대체 표지 |
| 1 | sc_fof03_hero | E | 1200×800 | 새로 | P2 | 히어로 무대(선택) | 표지 |
| 2 | doc_think · asst_smile · fly_point · robo_coin | A~D | 96 | 재사용 | — | 히어로 대화창 | — |
| 3 | fly_point · robo_coin | C·D | 96 | 재사용 | — | 대결 전 | — |
| 4 | fly_arms · robo_sigh · asst_firm · doc_judge | C·D·B·A | 96 | 재사용 | — | 대결 후 (F) | — |
| 5 | cut_fof03_lv5 | G | 960×540 | 새로 | P1 | ⑤칸 컷 | 없음(지도 캔버스가 같은 내용) |
| 6 | sc_fof03_outro | E | 1200×800 | 새로 | P2 | 아웃트로 | 표지 |
| 7 | thumb_fof03 | I | 600×400 | 새로 (표지 3:2 자르기) | P3 | 목차 카드 | 색 카드 |
| 8 | og_fof03 | K | 1200×630 | 새로 (표지 자르기) | P3 | 공유 미리보기 | 없음 |

## 3. 새로 그릴 그림 상세

### 3-1. `cut_fof03_lv5` — 짐을 진 승객으로 붐비는 환승 통로
| 항목 | 내용 |
|---|---|
| 판 · 크기 | G · 960×540 |
| 구도 | 축소 모형 환승 통로에 작은 빛 상자를 여러 개 겹쳐 실은 수레들이 몰려 있다(레버리지 은유). 초파리가 왼쪽에서 오른쪽을 보며 돋보기와 체크보드로 통로를 점검한다 |
| 표정·몸짓 | 초파리 fly_magnify 계열 |
| 소품 | 축소 모형 통로, 짐을 높이 실은 수레(사람 없음), 경고등 없는 노란 빛 |
| 피할 것 | 글자, 숫자, 실제 회사·지하철 로고, 사고 장면 |
| 대체 글 (alt) | 초파리 연구원이 무거운 짐을 진 승객으로 붐비는 환승 통로를 점검하는 장면 |

**프롬프트 (복사해서 사용)**
```
16-bit RPG style pixel art, bold dark outline, 2–3 tone shading, small highlights, consistent with the reference images, cozy night laboratory mood, purple light, soft magenta and green fluorescent accents, 16:9 illustration panel, a tabletop miniature transit corridor crowded with tiny carts each carrying tall stacks of glowing boxes, warm yellow light, anthropomorphic fruit fly researcher, black body, big red compound eyes, blue helmet with a gold stripe and pink and blue cables, white lab coat over a black vest, black gloves, transparent wings, on the left facing right inspecting the corridor with a magnifying glass, the stacked carts are the brightest spot, no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands
```

### 3-2. `sc_fof03_outro` — 결과 후 넷 (F)
| 항목 | 내용 |
|---|---|
| 판 · 크기 | E · 1200×800 |
| 구도 | 승자 초파리가 앞쪽 왼쪽에서 팔짱을 끼고 뿌듯한 표정(fly_arms), 주판봇은 오른쪽 뒤에서 나무 주판을 내리고 가볍게 한숨(robo_sigh, 조롱 없이). 박사는 가운데 뒤에서 한 줄로만 이어진 역들을 가리키고, 조수는 옆에서 장부를 들고 눈을 반짝인다 |
| 피할 것 | 조롱하는 몸짓, 글자 |
| 대체 글 (alt) | 대결이 끝난 뒤 네 캐릭터가 정거장 지도 앞에 모인 장면 |
| 대신 쓰는 그림 | 표지 |

**프롬프트 (복사해서 사용)**
```
16-bit RPG style pixel art, bold dark outline, 2–3 tone shading, small highlights, consistent with the reference images, cozy night laboratory mood, purple light, soft magenta and green fluorescent accents, 3:2 landscape scene, medium brightness, in front of a tabletop miniature of transit stations, one row of stations linked in a single line has tipped over like dominoes, boxy beige retro CRT-monitor robot, dark green screen face with mint pixel eyes and mouth, short antenna topped with a red-brown abacus bead, gray segmented arms, two small tank treads, in the front left facing right, arms crossed with a proud satisfied look, anthropomorphic fruit fly researcher, black body, big red compound eyes, blue helmet with a gold stripe and pink and blue cables, white lab coat over a black vest, black gloves, transparent wings, at the back right facing left, lowering a wooden abacus with a small good-natured sigh, chibi scientist, thin teal rectangular glasses, spiky black hair with one white streak, small ponytail at the back, white lab coat over black vest and tie, at the back center pointing at the toppled row of stations, girl researcher, long pink hair with two round buns and a navy streak, blue eyes, white lab coat over lavender hoodie, jeans, at the side holding a ledger with sparkling eyes, avoid for the robot: white glossy round head, black pill-shaped screen, yellow or golden eyes, round ball antenna knob, cyan chest light, floating or hovering, gold coins, no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands
```

### 3-3. `sc_fof03_hero` — 선택
표지와 같은 장소에서 네 캐릭터가 환승역 모형을 올려다보는 3:2 장면. 표지가 있으면 만들지 않아도 된다(P2).

## 4. 일관성 지침
- 참고 이미지: `adminmrobo/fruitfly-lab-expressions` 기본 그림 4장 (로봇은 `images/jupanbot/`의 주판봇)
- 주판봇 검수: 흰 둥근 머리 · 검은 알약형 화면 · 노란 눈 · 공 모양 안테나 · 시안 가슴 등 · 공중 부유 · 금화가 보이면 회사 캐릭터(Money-Robo)가 섞인 것이므로 다시 생성
- 같은 캐릭터는 같은 세션에서, 시드를 고정할 수 있으면 고정
- 01·02편과 같은 연구실·조명을 쓰되 배관·실 그물 대신 환승역 모형으로 바꾼다
- 투명 배경이 안 되면: *solid flat #00ff00 background*

## 5. 넘겨받은 뒤 처리
1. 크기 확인, WebP 변환(표지 1600×900 220 KB 이하)
2. `data-img` 키 자리에 넣기: 표지는 `<!-- lab-cover -->` 블록 안의 캔버스를 `<picture>`로 바꾸고, 컷은 `hidden`을 지운다
3. 페이지 크기: 현재 약 250 KB. 표지 220 KB를 넣어도 600 KB 기준 안
4. 390·768·1280 폭에서 얼굴 잘림 확인

## 6. 체크리스트
- [x] 결과 전 그림(표지)에 승패 암시 없음
- [x] 모든 프롬프트에 고정 외형과 금지 구절
- [x] 그림 안 글자 없음, 실존 브랜드 없음

## 7. 매니페스트
```json
{
  "page": "03_fof_between_stations",
  "anchor": "D:transit-stations",
  "season": "default",
  "duel": {"result": "F", "gap": 1},
  "images": [
    {"key":"cover_fof03","plate":"L","size":[1920,1080],"status":"new","priority":"P1","slot":"cover","fallback":"canvas-five-stations","alt":"밤의 연구실에서 네 캐릭터가 서로 줄로 이어진 정거장 다섯 곳을 살피는 표지"},
    {"key":"cut_fof03_lv5","plate":"G","size":[960,540],"status":"new","priority":"P1","slot":"lv5","fallback":"none","alt":"초파리 연구원이 물류센터 같은 은행 상자를 열어 안쪽 분류 선반을 들여다보는 장면"},
    {"key":"sc_fof03_outro","plate":"E","size":[1200,800],"status":"new","priority":"P2","slot":"outro","fallback":"cover_fof03","alt":"대결이 끝난 뒤 네 캐릭터가 정거장 지도 앞에 모인 장면"},
    {"key":"sc_fof03_hero","plate":"E","size":[1200,800],"status":"new","priority":"P2","slot":"hero-stage","fallback":"cover_fof03","alt":"네 캐릭터가 줄로 이어진 정거장 다섯 곳을 올려다보는 장면"},
    {"key":"thumb_fof03","plate":"I","size":[600,400],"status":"new","priority":"P3","slot":"index-card","fallback":"color-card","alt":"금융기관끼리 표지 축소판"},
    {"key":"og_fof03","plate":"K","size":[1200,630],"status":"new","priority":"P3","slot":"og","fallback":"none","alt":"금융기관끼리 공유 미리보기"},
    {"key":"fly_arms","plate":"C","size":[96,96],"status":"reuse","slot":"duel-after","fallback":"fly_clip","alt":""},
    {"key":"robo_sigh","plate":"D","size":[96,96],"status":"reuse","slot":"duel-after","fallback":"robo_smile","alt":""}
  ]
}
```
