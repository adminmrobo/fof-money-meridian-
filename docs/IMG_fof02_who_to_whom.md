# 02번 「누가 누구에게 — 상세자금순환표로 그리는 돈의 지도」 이미지 제작 명세서

> **그림 반영 (2026-11-07):** 표지·목차 카드·공유 미리보기·본문 컷·아웃트로 그림을 받아 저장소 루트에 WebP/JPG로 올리고 페이지에 넣었다. 히어로 무대 컷(`sc_fof02_hero`)은 선택 항목이라 아직 숨김 상태다.

| 항목 | 내용 |
|---|---|
| 페이지 | 02_fof_who_to_whom.html |
| 모드 / 주 앵커 | 교과서 모드 / D 생활·현장: 연구실의 실 그물(부문 연결), 보조 C 장부 |
| 시즌 | 기본 |
| 대결 | 장난감 경제에서 예금 10이 펀드로 가고 은행이 기업대출 비중을 줄이면 기업 몫이 커지나 → 결과 R (주판봇 승, 39 → 32) |
| 새로 그릴 그림 | P1 2장 · P2 2장 · P3 2장 |
| 재사용 | 표정 18장 (캐릭터 팩 96px, 페이지에 base64로 들어 있음) |
| 그림이 없을 때 | 표지는 캔버스 대체 표지(색 구슬 일곱 + 실 그물 + 캐릭터 넷), 나머지 칸은 숨김 상태라 페이지는 완성 상태 |

## 1. 그림체와 고정 외형
- 스타일: SKILL 18-3 (16비트 RPG 픽셀아트, 굵은 외곽선, 2~3단계 명암)
- 캐릭터 고정 외형: 캐릭터 팩 18-4 그대로
- 이 페이지 장소: 밤의 연구실에 걸린 실 그물, 일곱 색 구슬(가계 분홍·은행 하늘·보험 보라·펀드 자홍·기업 청록·정부 금색·해외 산호)
- 장소 영어 묘사: *a night laboratory with seven glowing colored orbs hanging in the air, connected by thin luminous threads like a web*

## 2. 필요한 그림 전체

| # | 키 | 판 | 크기 | 상태 | 우선 | 들어가는 곳 | 대신 쓰는 그림 |
|---|---|---|---|---|---|---|---|
| 0 | cover_fof02 | L | 1920×1080 | 새로 (COVER_fof02_who_to_whom.md) | P1 | 맨 위 글 표지 | 캔버스 대체 표지 |
| 1 | sc_fof02_hero | E | 1200×800 | 새로 | P2 | 히어로 무대(선택) | 표지 |
| 2 | doc_think · asst_smile · fly_point · robo_coin | A~D | 96 | 재사용 | — | 히어로 대화창 | — |
| 3 | fly_point · robo_coin | C·D | 96 | 재사용 | — | 대결 전 | — |
| 4 | fly_coffee · robo_happy · asst_firm · doc_judge | C·D·B·A | 96 | 재사용 | — | 대결 후 (R) | — |
| 5 | cut_fof02_lv5 | G | 960×540 | 새로 | P1 | ⑤칸 컷 | 없음(지도 캔버스가 같은 내용) |
| 6 | sc_fof02_outro | E | 1200×800 | 새로 | P2 | 아웃트로 | 표지 |
| 7 | thumb_fof02 | I | 600×400 | 새로 (표지 3:2 자르기) | P3 | 목차 카드 | 색 카드 |
| 8 | og_fof02 | K | 1200×630 | 새로 (표지 자르기) | P3 | 공유 미리보기 | 없음 |

## 3. 새로 그릴 그림 상세

### 3-1. `cut_fof02_lv5` — 은행 상자 속 분류 선반
| 항목 | 내용 |
|---|---|
| 판 · 크기 | G · 960×540 |
| 구도 | 하늘색으로 빛나는 큰 상자(은행)의 뚜껑이 열려 있고, 안쪽에 색 구슬들이 여러 선반(청록·분홍·금색)으로 나뉘어 담겨 있다. 초파리가 왼쪽에서 오른쪽을 보며 돋보기로 선반을 들여다본다 |
| 표정·몸짓 | 초파리 fly_magnify 계열 |
| 소품 | 뚜껑 열린 상자, 색 선반, 상자로 들어오는 실 한 가닥과 나가는 실 여러 가닥 |
| 피할 것 | 글자, 숫자, 실제 은행 로고 |
| 대체 글 (alt) | 초파리 연구원이 물류센터 같은 은행 상자를 열어 안쪽 분류 선반을 들여다보는 장면 |

**프롬프트 (복사해서 사용)**
```
16-bit RPG style pixel art, bold dark outline, 2–3 tone shading, small highlights, consistent with the reference images, cozy night laboratory mood, purple light, soft magenta and green fluorescent accents, 16:9 illustration panel, a large glowing light-blue box with its lid open, inside it colored beads sorted onto several shelves (teal, pink, gold), one luminous thread entering the box and several threads leaving it toward distant orbs, anthropomorphic fruit fly researcher, black body, big red compound eyes, blue helmet with a gold stripe and pink and blue cables, white lab coat over a black vest, black gloves, transparent wings, on the left facing right peering into the shelves through a magnifying glass, the open box is the brightest spot, no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands
```

### 3-2. `sc_fof02_outro` — 결과 후 넷 (R)
| 항목 | 내용 |
|---|---|
| 판 · 크기 | E · 1200×800 |
| 구도 | 승자 주판봇이 앞쪽 오른쪽에서 나무 주판을 들고 웃고(robo_happy), 초파리는 왼쪽에서 커피잔을 들고 인정하는 몸짓(fly_coffee). 박사는 가운데 뒤에서 실 그물의 가장 굵은 실을 가리키고, 조수는 옆에서 장부를 들고 눈을 반짝인다 |
| 피할 것 | 조롱하는 몸짓, 글자 |
| 대체 글 (alt) | 대결이 끝난 뒤 네 캐릭터가 실 그물 앞에 모인 장면 |
| 대신 쓰는 그림 | 표지 |

**프롬프트 (복사해서 사용)**
```
16-bit RPG style pixel art, bold dark outline, 2–3 tone shading, small highlights, consistent with the reference images, cozy night laboratory mood, purple light, soft magenta and green fluorescent accents, 3:2 landscape scene, medium brightness, in front of a web of luminous threads connecting seven glowing colored orbs, one thread much thicker than the others, boxy beige retro CRT-monitor robot, dark green screen face with mint pixel eyes and mouth, short antenna topped with a red-brown abacus bead, gray segmented arms, two small tank treads, on the left facing right, holding a coffee cup with a small accepting shrug, anthropomorphic fruit fly researcher, black body, big red compound eyes, blue helmet with a gold stripe and pink and blue cables, white lab coat over a black vest, black gloves, transparent wings, in the front right facing left, happy mint pixel eyes, raising a wooden abacus, chibi scientist, thin teal rectangular glasses, spiky black hair with one white streak, small ponytail at the back, white lab coat over black vest and tie, at the back center pointing at the thickest thread, girl researcher, long pink hair with two round buns and a navy streak, blue eyes, white lab coat over lavender hoodie, jeans, at the side holding a ledger with sparkling eyes, avoid for the robot: white glossy round head, black pill-shaped screen, yellow or golden eyes, round ball antenna knob, cyan chest light, floating or hovering, gold coins, no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands
```

### 3-3. `sc_fof02_hero` — 선택
표지와 같은 장소에서 네 캐릭터가 실 그물을 올려다보는 3:2 장면. 표지가 있으면 만들지 않아도 된다(P2).

## 4. 일관성 지침
- 참고 이미지: `adminmrobo/fruitfly-lab-expressions` 기본 그림 4장 (로봇은 `images/jupanbot/`의 주판봇)
- 주판봇 검수: 흰 둥근 머리 · 검은 알약형 화면 · 노란 눈 · 공 모양 안테나 · 시안 가슴 등 · 공중 부유 · 금화가 보이면 회사 캐릭터(Money-Robo)가 섞인 것이므로 다시 생성
- 같은 캐릭터는 같은 세션에서, 시드를 고정할 수 있으면 고정
- 01편과 같은 연구실·조명을 쓰되 배관 대신 실 그물로 바꾼다
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
  "page": "02_fof_who_to_whom",
  "anchor": "D:thread-web",
  "season": "default",
  "duel": {"result": "R", "gap": 7},
  "images": [
    {"key":"cover_fof02","plate":"L","size":[1920,1080],"status":"new","priority":"P1","slot":"cover","fallback":"canvas-thread-web","alt":"밤의 연구실에서 네 캐릭터가 부문과 부문을 잇는 실 그물을 따라가는 표지"},
    {"key":"cut_fof02_lv5","plate":"G","size":[960,540],"status":"new","priority":"P1","slot":"lv5","fallback":"none","alt":"초파리 연구원이 물류센터 같은 은행 상자를 열어 안쪽 분류 선반을 들여다보는 장면"},
    {"key":"sc_fof02_outro","plate":"E","size":[1200,800],"status":"new","priority":"P2","slot":"outro","fallback":"cover_fof02","alt":"대결이 끝난 뒤 네 캐릭터가 실 그물 앞에 모인 장면"},
    {"key":"sc_fof02_hero","plate":"E","size":[1200,800],"status":"new","priority":"P2","slot":"hero-stage","fallback":"cover_fof02","alt":"네 캐릭터가 부문 사이를 잇는 실 그물을 올려다보는 장면"},
    {"key":"thumb_fof02","plate":"I","size":[600,400],"status":"new","priority":"P3","slot":"index-card","fallback":"color-card","alt":"누가 누구에게 표지 축소판"},
    {"key":"og_fof02","plate":"K","size":[1200,630],"status":"new","priority":"P3","slot":"og","fallback":"none","alt":"누가 누구에게 공유 미리보기"},
    {"key":"fly_coffee","plate":"C","size":[96,96],"status":"reuse","slot":"duel-after","fallback":"fly_clip","alt":""},
    {"key":"robo_happy","plate":"D","size":[96,96],"status":"reuse","slot":"duel-after","fallback":"robo_smile","alt":""}
  ]
}
```
