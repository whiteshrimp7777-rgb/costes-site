# Design System: COSTES — co's tes
**Brand:** co's tes (cowarrr의 너의 것들)
**Product:** 슈팅스타 TradingView 인디케이터

## 1. Visual Theme & Atmosphere

COSTES는 **"The Golden Terminal"** — 기관급 트레이딩 터미널의 냉철한 정밀함 위에 골드 액센트가 빛나는 프리미엄 다크 인터페이스. @cowarrr이 52만 달러 수익을 만든 지표를 판매하는 사이트답게, 인터페이스 자체가 "이 도구를 쓰면 돈을 번다"는 확신을 심어주어야 한다.

분위기는 **냉철하면서도 대담한(Cold yet Bold)** — 울트라 다크 배경 위에 골드 액센트가 고급 시계나 프리미엄 트레이딩 데스크처럼 빛난다. 모든 UI 요소는 "기관 트레이더의 전용 터미널"이라는 느낌을 전달해야 한다.

**핵심 특성:**
- 울트라 다크 배경 위의 골드 액센트가 만드는 럭셔리 트레이딩 무드
- 데이터가 "투영"되는 듯한 깊이감 있는 표면 계층화
- No-Line 규칙: 1px 보더 대신 배경색 톤 차이로 구역 분리
- 글래스모피즘과 골드 그라디언트의 조화
- 전문적 트레이딩 용어와 대담한 수익 어필의 균형
- 9개 시장(BTC, ETH, TSLA, NVDA, 삼성전자, SK하이닉스, 금, 원유, 환율)을 아우르는 범용성

## 2. Color Palette & Roles

### Primary Foundation
- **Obsidian Void** (#0c0c0e) — 메인 배경. 순수 블랙이 아닌 미세한 웜톤을 가진 울트라 다크. 골드 액센트가 최대한 빛나는 "무한한 어둠"의 캔버스.
- **Charcoal Abyss** (#121214) — 표면 1단계. 네비게이션 바, 사이드바 등 주요 구조 요소의 배경.
- **Gunmetal Slate** (#1a1a1e) — 표면 2단계. 카드, 컨테이너의 기본 배경.
- **Midnight Steel** (#242428) — 표면 3단계. 활성 카드, 호버 상태의 배경.
- **Smoke Iron** (#2e2e34) — 표면 4단계. 최상위 레이어, 드롭다운, 모달 배경.

### Gold Accent System (브랜드 시그니처)
- **Imperial Gold** (#F5C518) — 메인 액센트. CTA 버튼, 핵심 수치 강조, 활성 네비게이션에 사용. 사이트의 시그니처 컬러.
- **Radiant Amber** (#FFD700) — 밝은 골드. 호버 상태, 하이라이트, 배지에 사용.
- **Antique Brass** (#C9A200) — 진한 골드. 그라디언트의 끝점, 눌린 버튼 상태, 보조 액센트.

### Trading Signal Colors
- **Bullish Emerald** (#00E676) — 매수 시그널, 수익 표시, 긍정적 성과 지표.
- **Bearish Crimson** (#FF5252) — 매도 시그널, 손실 표시, 경고.

### Typography Colors
- **Pure White** (#FFFFFF) — 헤드라인, 핵심 수치, 강조 텍스트.
- **Silver Haze** (#B0B0B8) — 본문 텍스트, 설명문.
- **Graphite Mist** (#6B6B75) — 보조 텍스트, 메타데이터, 비활성 요소.

### The "No-Line" Rule
**명시적 지침:** 1px solid 보더로 섹션을 구분하지 않는다. 모든 레이아웃 경계는 배경색 차이로 표현한다. 사이드바는 `Charcoal Abyss`(#121214) 위에 `Obsidian Void`(#0c0c0e) 메인 배경과 대비시킨다. 선이 필요하다고 느끼면 톤 차이를 더 높인다.

### The Glass & Gradient Rule
- **CTA 버튼:** Imperial Gold(#F5C518)에서 Antique Brass(#C9A200)로의 135도 리니어 그라디언트. "녹은 금속" 느낌의 프리미엄 질감.
- **Lifetime 배너:** 위와 같은 골드 그라디언트를 넓은 배너에 적용. 15% 투명도로 배경에 깔아 "골든 글로우" 효과.
- **플로팅 모달:** Smoke Iron(#2e2e34)에 60% 투명도 + `backdrop-filter: blur(16px)`로 "프로스티드 옵시디언" 효과.

## 3. Typography Rules

**브랜드명:** "co's tes" — Pretendard SemiBold, letter-spacing: 0.08em
**한국어 본문:** Pretendard — 획에 꺾임이 없는 깔끔한 네오 고딕. 현대적이고 기술적인 느낌.
**영문/CTA:** Inter — 수학적 정밀함의 대명사. 트레이딩 업계 표준 폰트.
**데이터/숫자:** Space Grotesk — 티커 심볼, 가격, 수익률 등 "하드 데이터"에 사용.

### 계층 구조
- **Display (히어로 헤드라인):** Pretendard Bold, 3.5rem, letter-spacing: -0.02em. "52만 달러 수익을 만든, 단 하나의 시그널"
- **Headline (섹션 타이틀):** Pretendard SemiBold, 2.25rem, letter-spacing: -0.01em.
- **Title (카드 타이틀):** Pretendard Medium, 1.5rem.
- **Body (본문):** Pretendard Regular, 1rem, line-height: 1.7. 편안한 가독성.
- **Label (메타데이터):** Inter Medium, 0.75rem, uppercase, letter-spacing: 0.05em. 항공우주 계기판 느낌.
- **Data (수치):** Space Grotesk SemiBold, 가변 크기. 가격, 수익률, 퍼센트 등에 전용.

### 수익 강조 규칙
- 달러 수익($520,000)은 항상 Imperial Gold + Space Grotesk Bold로 표시
- 퍼센트 수익은 Bullish Emerald로 표시
- 마이너스 수치는 Bearish Crimson

## 4. Component Stylings

### Buttons
- **Primary CTA:** 골드 그라디언트(#F5C518 → #C9A200, 135도), 다크 텍스트(#0c0c0e), rounded-lg(8px), padding: 0.875rem 2.5rem. 호버 시 brightness(1.15) + 미세한 골드 글로우.
- **Secondary:** Gunmetal Slate(#1a1a1e) 배경, Imperial Gold(#F5C518) 텍스트, Ghost Border(Imperial Gold 15% 투명도).
- **Ghost:** 배경 없음, Silver Haze 텍스트, 호버 시 Midnight Steel 배경 페이드인.

### Cards & Containers
- **코너:** 12px(0.75rem) — 부드럽고 모던한 엣지.
- **배경:** Gunmetal Slate(#1a1a1e) 기본, 호버 시 Midnight Steel(#242428)로 전환.
- **그림자:** 기본 없음. 호버 시 Imperial Gold를 6% 투명도로 40px 블러 → "골든 글로우" 효과.
- **내부 패딩:** 2rem(32px).
- **No-Line 준수:** 보더 대신 배경 톤 차이로 구분.

### Pricing Cards
- **Standard:** Gunmetal Slate 배경. 깔끔하고 기능적.
- **Pro:** Midnight Steel 배경 + Imperial Gold 상단 스트라이프(3px). "POPULAR" 골드 배지.
- **Lifetime 배너:** 풀 너비, 골드 그라디언트 배경(15% 투명도) + 글래스모피즘.

### Navigation
- **스타일:** 가로 배치, 아이템 간 2.5rem 간격.
- **기본:** Silver Haze 텍스트.
- **활성/호버:** Imperial Gold로 부드러운 전환(200ms).
- **활성 인디케이터:** 하단 2px Imperial Gold 언더라인.
- **"co's tes" 브랜드:** 좌측 정렬, Pretendard SemiBold.

### Market Tags
- **스타일:** 알약 형태(rounded-full), Charcoal Abyss 배경, Silver Haze 텍스트.
- **아이콘:** 각 시장별 심볼 (₿, Ξ, TSLA, NVDA, 삼성, SK, Au, Oil, $/₩).

### FAQ Accordion
- **닫힌 상태:** Gunmetal Slate 배경, Silver Haze 질문 텍스트, 우측 + 아이콘.
- **열린 상태:** Midnight Steel 배경, Pure White 질문 텍스트, 본문은 Silver Haze.
- **구분:** 아이템 간 4px 간격(보더 아님).

## 5. Layout Principles

### Grid & Structure
- **최대 너비:** 1280px. 트레이딩 데이터 중심이므로 너무 넓지 않게.
- **그리드:** 12컬럼 반응형, gutters 24px(모바일) / 32px(데스크탑).
- **가격표:** 2컬럼 나란히(데스크탑), 1컬럼 스택(모바일).
- **브레이크포인트:** 모바일 <768px, 태블릿 768-1024px, 데스크탑 >1024px.

### Whitespace Strategy
- **베이스 유닛:** 8px.
- **섹션 간격:** 6-8rem(96-128px) — 극적인 여백으로 고급스러움 강조.
- **카드 내부:** 2rem(32px) 패딩.
- **히어로 상하:** 10rem — 임팩트 있는 첫 인상.

### Responsive
- 모바일 퍼스트 설계
- 가격표: 데스크탑 2컬럼 → 모바일 1컬럼 스택
- 시장 태그: 가로 스크롤
- 히어로 텍스트: 모바일에서 2.25rem으로 축소
- 터치 타겟: 최소 44x44px

## 6. Design System Notes for Stitch Generation

### 핵심 프롬프트 언어
- **분위기:** "기관급 트레이딩 터미널의 냉철한 골든 프리미엄"
- **버튼:** "녹은 금속 질감의 골드 그라디언트"
- **그림자:** "골든 글로우 — 6% 투명도의 은은한 금빛 발광"
- **간격:** "극적인 여백으로 고급스러움 강조"
- **데이터:** "항공우주 계기판의 정밀한 데이터 표시"

### 컬러 참조
- Primary CTA: "Imperial Gold (#F5C518)"
- 배경: "Obsidian Void (#0c0c0e)" 또는 "Gunmetal Slate (#1a1a1e)"
- 텍스트: "Pure White (#FFFFFF)" 또는 "Silver Haze (#B0B0B8)"
- 수익: "Imperial Gold + Space Grotesk Bold"

### 핵심 카피
- 히어로: "52만 달러 수익을 만든, 단 하나의 시그널"
- 서브: "@cowarrr이 직접 설계한 기관급 트레이딩 인디케이터"
- 가치: "저위험 진입 · 고수익 청산 · 정밀 타이밍"
- CTA: "슈팅스타로 시작하기"
- Lifetime: "한 번의 결제, 영원한 엣지"
