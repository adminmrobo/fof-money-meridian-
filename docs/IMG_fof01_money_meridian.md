# 01번 「돈의 경맥 — 경제순환에서 자금순환표까지」 이미지 제작 명세서

> **그림 반영 (2026-11-07):** 표지·목차 카드·공유 미리보기·본문 컷·아웃트로 그림을 받아 저장소 루트에 WebP/JPG로 올리고 페이지에 넣었다. 히어로 무대 컷(`sc_fof01_hero`)은 선택 항목이라 아직 숨김 상태다.

| 항목 | 내용 |
|---|---|
| 페이지 | 01_fof_money_meridian.html |
| 모드 / 주 앵커 | 교과서 모드 / D 생활·현장: 연구실 벽의 배관망(경맥), 보조 C 장부(회계 다리) |
| 시즌 | 기본 |
| 대결 | 시나리오 기본값에서 소득 경로가 자산 경로를 넘는 환류율은 4%면 충분한가 → 결과 R (주판봇 승, 문턱 약 3.2%) |
| 새로 그릴 그림 | P1 2장 · P2 3장 · P3 2장 |
| 재사용 | 표정 18장 (캐릭터 팩 96px, 페이지에 base64로 들어 있음) |
| 그림이 없을 때 | 표지는 캔버스 대체 표지(관 네 줄 + 캐릭터 넷), 나머지는 이미 완성 상태 |

## 1. 그림체와 고정 외형
- 스타일: SKILL 18-3 (16비트 RPG 픽셀아트, 굵은 외곽선, 2~3단계 명암)
- 캐릭터 고정 외형: 캐릭터 팩 18-4 그대로
- 이 페이지 장소: 밤의 연구실 벽을 덮은 투명 배관망, 네 색 관(가계 분홍·기업 청록·정부 하늘·국외 산호), 관 속을 흐르는 빛 구슬
- 장소 영어 묘사: *a night laboratory whose back wall is covered by a network of transparent glass pipes in four colors, glowing beads flowing inside, purple lab light from one side*

## 2. 필요한 그림 전체

| # | 키 | 판 | 크기 | 상태 | 우선 | 들어가는 곳 | 대신 쓰는 그림 |
|---|---|---|---|---|---|---|---|
| 0 | cover_fof01 | L | 1920×1080 | 새로 (COVER_fof01_money_meridian.md) | P1 | 맨 위 글 표지 | 캔버스 대체 표지 |
| 1 | sc_fof01_hero | E | 1200×800 | 새로 | P2 | 히어로 무대(선택) | 표지 |
| 2 | doc_think · asst_smile · fly_point · robo_coin | A~D | 96 | 재사용 | — | 히어로 대화창 | — |
| 3 | fly_point · robo_calc · asst_report · fly_magnify | C·D·B | 96 | 재사용 | — | 본문 말풍선 | — |
| 4 | fly_point · robo_coin | C·D | 96 | 재사용 | — | 대결 전 | — |
| 5 | fly_coffee · robo_happy · asst_firm · doc_judge | C·D·B·A | 96 | 재사용 | — | 대결 후 (R) | — |
| 6 | cut_fof01_lv4 | G | 960×540 | 새로 | P1 | ④ 회계 다리: 세 장부 컷 | 없음(표로 대신) |
| 7 | cut_fof01_lv5 | G | 960×540 | 새로 | P2 | ⑤ 저수지 컷 | 없음 |
| 8 | sc_fof01_outro | E | 1200×800 | 새로 | P2 | 아웃트로 | 표지 |
| 9 | thumb_fof01 | I | 600×400 | 새로 (표지 3:2 자르기) | P3 | 목차 카드 | 색 카드 |
| 10 | og_fof01 | K | 1200×630 | 새로 (표지 자르기) | P3 | 공유 미리보기 | 없음 |
| — | 시뮬레이션 캔버스 | — | — | 코드 | — | 캔버스 2D | — |

## 3. 새로 그릴 그림 상세

### 3-1. `cut_fof01_lv4` — 세 장부를 펼친 박사와 조수
| 항목 | 내용 |
|---|---|
| 판 · 크기 | G · 960×540 |
| 배경 | 그림 전체 |
| 구도 | 책상 위에 큰 장부 세 권(빈 줄무늬 쪽)이 펼쳐져 있고, 세 장부에서 나온 빛줄기가 벽의 배관망으로 이어진다. 박사는 가운데 장부를 가리키고, 조수는 옆에서 장부를 넘긴다 |
| 표정·몸짓 | 박사 doc_front 계열, 조수 asst_report 계열 |
| 소품 | 장부 세 권(글자 없음, 색 띠로만 구분: 노랑·청록·분홍), 벽의 배관 |
| 빛·분위기 | 장부에서 올라오는 부드러운 빛 |
| 피할 것 | 장부 속 글자·숫자, 실제 회사 로고 |
| 대체 글 (alt) | 박사와 조수가 펼쳐진 장부 세 권에서 벽의 관으로 이어지는 빛줄기를 살펴보는 장면 |
| 대신 쓰는 그림 | 없음 (대응표가 같은 내용을 글로 보여 줌) |

**프롬프트 (복사해서 사용)**
```
16-bit RPG style pixel art, bold dark outline, 2–3 tone shading, small highlights, consistent with the reference images, cozy night laboratory mood, purple light, soft magenta and green fluorescent accents, 16:9 illustration panel, chibi scientist, thin teal rectangular glasses, spiky black hair with one white streak, small ponytail at the back, white lab coat over black vest and tie, pointing at the middle of three large open ledgers with blank striped pages on a lab desk, girl researcher, long pink hair with two round buns and a navy streak, blue eyes, white lab coat over lavender hoodie, jeans, turning a page beside him, soft beams of light rising from the three ledgers (yellow, teal, pink bands) into a network of glass pipes on the wall, no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands
```

### 3-2. `cut_fof01_lv5` — 흐르는 관과 부푼 저수지
| 항목 | 내용 |
|---|---|
| 판 · 크기 | G · 960×540 |
| 배경 | 그림 전체 |
| 구도 | 왼쪽에서 가는 관(초록 구슬, '거래')이 들어와 큰 유리 수조로 이어지는데, 수조 안 금빛 액체는 관에서 들어온 양보다 훨씬 많이 부풀어 있다. 초파리가 왼쪽에서 오른쪽을 보며 돋보기로 수조를 들여다본다 |
| 표정·몸짓 | 초파리 fly_magnify 계열 |
| 소품 | 유리 수조, 눈금(숫자 없음), 가는 관 |
| 빛·분위기 | 수조의 금빛이 화면에서 가장 밝다 |
| 피할 것 | 눈금 숫자, 실제 지수·종목 기호 |
| 대체 글 (alt) | 가는 관으로 조금 들어온 구슬보다 훨씬 크게 부풀어 오른 금빛 수조를 초파리 연구원이 돋보기로 살피는 장면 |
| 대신 쓰는 그림 | 없음 (저수지 막대 그래프가 같은 내용) |

**프롬프트 (복사해서 사용)**
```
16-bit RPG style pixel art, bold dark outline, 2–3 tone shading, small highlights, consistent with the reference images, cozy night laboratory mood, purple light, soft magenta and green fluorescent accents, 16:9 illustration panel, a thin glass pipe carrying a few green glowing beads flows from the left into a large glass tank whose golden liquid is swollen far above the pipe's level, gauge marks without numbers, anthropomorphic fruit fly researcher, black body, big red compound eyes, blue helmet with a gold stripe and pink and blue cables, white lab coat over a black vest, black gloves, transparent wings, on the left facing right peering into the tank through a magnifying glass, the golden tank is the brightest spot, no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands
```

### 3-3. `sc_fof01_outro` — 결과 후 넷
| 항목 | 내용 |
|---|---|
| 판 · 크기 | E · 1200×800 |
| 구도 | 승자 주판봇이 앞쪽 오른쪽에서 나무 주판을 들고 웃고(robo_happy), 초파리는 왼쪽 뒤에서 커피잔을 들고 인정하는 몸짓(fly_coffee). 박사는 가운데 뒤에서 세 장부를 들고, 조수는 옆에서 웃는다 |
| 피할 것 | 조롱하는 몸짓, 글자 |
| 대체 글 (alt) | 대결이 끝난 뒤 나무 주판을 든 주판봇과 커피잔을 든 초파리 연구원, 장부를 든 박사와 웃는 조수가 배관망 앞에 모인 장면 |
| 대신 쓰는 그림 | 표지 |

**프롬프트 (복사해서 사용)**
```
16-bit RPG style pixel art, bold dark outline, 2–3 tone shading, small highlights, consistent with the reference images, cozy night laboratory mood, purple light, soft magenta and green fluorescent accents, 3:2 landscape scene, medium brightness, in front of a wall of transparent glass pipes with glowing beads, boxy beige retro CRT-monitor robot, dark green screen face with mint pixel eyes and mouth, short antenna topped with a red-brown abacus bead, gray segmented arms, two small tank treads, in the front right facing left, happy mint pixel eyes, raising a wooden abacus, anthropomorphic fruit fly researcher, black body, big red compound eyes, blue helmet with a gold stripe and pink and blue cables, white lab coat over a black vest, black gloves, transparent wings, on the left facing right, half-closed relaxed eyes, holding a coffee cup with a small accepting shrug, chibi scientist, thin teal rectangular glasses, spiky black hair with one white streak, small ponytail at the back, white lab coat over black vest and tie, at the back center holding three closed ledgers, girl researcher, long pink hair with two round buns and a navy streak, blue eyes, white lab coat over lavender hoodie, jeans, smiling at the side, avoid for the robot: white glossy round head, black pill-shaped screen, yellow or golden eyes, round ball antenna knob, cyan chest light, floating or hovering, gold coins, no text, no letters, no numbers, no logos, no weapons, no cigarettes, no alcohol, no blood, no real brands
```

### 3-4. `sc_fof01_hero` — 선택
표지와 같은 장소에서 네 캐릭터가 관을 올려다보는 3:2 장면. 표지가 있으면 만들지 않아도 된다(P2).

## 4. 일관성 지침
- 참고 이미지: `adminmrobo/fruitfly-lab-expressions` 기본 그림 4장 (로봇은 `images/jupanbot/`의 주판봇)
- 주판봇 검수: 흰 둥근 머리 · 검은 알약형 화면 · 노란 눈 · 공 모양 안테나 · 시안 가슴 등 · 공중 부유 · 금화가 보이면 회사 캐릭터(Money-Robo)가 섞인 것이므로 다시 생성
- 같은 캐릭터는 같은 세션에서, 시드를 고정할 수 있으면 고정
- 표정만 바꿀 때: *same character, same size and position, only change the facial expression and pose to ...*
- 투명 배경이 안 되면: *solid flat #00ff00 background*

## 5. 넘겨받은 뒤 처리
1. 크기 확인, WebP 변환(표지 1600×900 220 KB 이하)
2. `data-img` 키 자리에 넣기: 표지는 `<!-- lab-cover -->` 블록 안의 캔버스를 `<picture>`로 바꾼다
3. 페이지 그림 합계: 현재 페이지 약 293 KB(표정 그림 약 120 KB 포함). 표지 220 KB를 넣으면 약 515 KB로 600 KB 기준 안
4. 390·768·1280 폭에서 얼굴 잘림 확인

## 6. 체크리스트
- [x] 결과 전 그림(표지)에 승패 암시 없음
- [x] 모든 프롬프트에 고정 외형과 금지 구절
- [x] 생물 앵커가 아니므로 현미경·해부 소품 없음
- [x] 그림 안 글자 없음, 실존 브랜드 없음
- [x] P1 2장 (표지 제외 1장)

## 7. 매니페스트
```json
{
  "page": "01_fof_money_meridian",
  "anchor": "D:pipe-network",
  "season": "default",
  "duel": {"result": "R", "gap": null},
  "images": [
    {"key":"cover_fof01","plate":"L","size":[1920,1080],"status":"new","priority":"P1","slot":"cover","fallback":"canvas-pipes-four","alt":"밤의 연구실에서 네 캐릭터가 돈이 흐르는 관과 한가운데 금빛으로 부푼 막힌 곳을 들여다보는 표지"},
    {"key":"cut_fof01_lv4","plate":"G","size":[960,540],"status":"new","priority":"P1","slot":"lv4","fallback":"none","alt":"박사와 조수가 펼쳐진 장부 세 권에서 벽의 관으로 이어지는 빛줄기를 살펴보는 장면"},
    {"key":"cut_fof01_lv5","plate":"G","size":[960,540],"status":"new","priority":"P2","slot":"lv5","fallback":"none","alt":"가는 관으로 조금 들어온 구슬보다 훨씬 크게 부풀어 오른 금빛 수조를 초파리 연구원이 돋보기로 살피는 장면"},
    {"key":"sc_fof01_outro","plate":"E","size":[1200,800],"status":"new","priority":"P2","slot":"outro","fallback":"cover_fof01","alt":"대결이 끝난 뒤 네 캐릭터가 배관망 앞에 모인 장면"},
    {"key":"sc_fof01_hero","plate":"E","size":[1200,800],"status":"new","priority":"P2","slot":"hero-stage","fallback":"cover_fof01","alt":"네 캐릭터가 연구실 벽의 관을 올려다보는 장면"},
    {"key":"thumb_fof01","plate":"I","size":[600,400],"status":"new","priority":"P3","slot":"index-card","fallback":"color-card","alt":"돈의 경맥 표지 축소판"},
    {"key":"og_fof01","plate":"K","size":[1200,630],"status":"new","priority":"P3","slot":"og","fallback":"none","alt":"돈의 경맥 공유 미리보기"},
    {"key":"fly_coffee","plate":"C","size":[96,96],"status":"reuse","slot":"duel-after","fallback":"fly_clip","alt":""},
    {"key":"robo_happy","plate":"D","size":[96,96],"status":"reuse","slot":"duel-after","fallback":"robo_smile","alt":""}
  ]
}
```
