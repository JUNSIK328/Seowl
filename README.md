# Seowl
Seoul never sleeps, and neither does Seowl.

작성하신 **Seowl 프로젝트 기획안을 이 'Agency-Agents' 환경에 100% 활용하는 완벽한 워크플로우와 명령어(프롬프트)**를 안내해 드립니다.

💡 핵심 세팅: Seowl 프로젝트 컨텍스트 파일 만들기

이 에이전트들은 지시받은 역할은 잘 수행하지만, '무엇을 만들지(Context)'는 알지 못합니다. 따라서 앞서 정리한 요약본을 작업 환경(VS Code, Cursor 등)의 최상위 폴더에 seowl_context.md (또는 project_brief.md)라는 파일로 저장해 둡니다.

*에이전트들이 작업할 때마다 **"seowl_context.md 파일을 읽고 이 프로젝트의 목적에 맞게 작업해 줘"*라고 지시하기 위함입니다.

🦉 Seowl을 위한 '에이전트별' 특화 프롬프트

Cursor, Claude CLI 등에서 각 에이전트를 활성화(Activate)하고 Seowl 맞춤형 지시를 내리는 방식입니다.

1. 기획 및 디자인 세팅 (Design Division)

① UI 디자이너 (UI Designer) & 브랜드 가디언 (Brand Guardian)

프롬프트:

"Activate UI Designer mode.
@seowl_context.md 문서를 먼저 완벽히 숙지해 줘.
우리는 '다크 모드' 중심의 심야 앱을 만들 거야. 유저의 피로도를 낮추면서도 트렌디한 타이포그래피와 네온 컬러 코드를 활용한 디자인 시스템(Color Palette, Typography, Button System)을 마크다운 표 형태로 정의해 줘."

② 윔지 인젝터 (Whimsy Injector) - 개성 부여 에이전트

프롬프트:

"Activate Whimsy Injector mode.
앱을 켰을 때와 로딩 중일 때 표시될 유머러스하고 매력적인 마이크로카피(Microcopy)를 기획해 줘. 앱 컨셉인 '잠들지 않는 부엉이'에 맞춰서 친근하고 재치 있는 문구를 화면별로 3개씩 제안해 줘."

2. 프론트엔드 및 앱 개발 (Engineering Division)

③ 모바일 앱 빌더 (Mobile App Builder)

프롬프트:

"Activate Mobile App Builder mode.
@seowl_context.md의 'Mobility-Mix' 기능에 명시된 운전자/뚜벅이 모드 토글 기능을 구현할 거야. React Native(또는 Flutter)를 사용해서 메인 지도 화면과 하단 바(Bottom Navigation), 그리고 모드를 전환하는 토글 스위치 버튼에 대한 기본 레이아웃 보일러플레이트(Boilerplate) 코드를 작성해 줘."

④ 프론트엔드 디벨로퍼 (Frontend Developer)

프롬프트:

"Activate Frontend Developer mode.
앱의 핵심인 '올빼미 필터(안심 지수, 콘센트 위치 등)'를 사용자가 직관적으로 껐다 켰다 할 수 있는 필터 칩(Filter Chip) 컴포넌트를 만들어줘. 부드러운 애니메이션(Framer Motion/Reanimated)이 적용되어야 하고 컴포넌트는 재사용 가능해야 해."

3. 백엔드 및 데이터베이스 (Engineering Division)

⑤ 데이터베이스 옵티마이저 (Database Optimizer)

프롬프트:

"Activate Database Optimizer mode.
@seowl_context.md에서 설명하는 'Proof of Life (실시간 생존 신고)' 기능을 위한 DB 스키마를 최적화해 줘. 읽기와 쓰기가 새벽 시간에 폭증할 텐데, 매장의 실시간 상태(영업 여부, 혼잡도)를 캐싱하고 관리하기 적합한 PostgreSQL과 Redis 아키텍처 구조를 설계하고 SQL 테이블 생성 쿼리를 작성해 줘."

⑥ 백엔드 아키텍트 (Backend Architect)

프롬프트:

"Activate Backend Architect mode.
특정 핫스팟(북악스카이웨이 등) 반경 1km 내에 있는 유저들끼리만 채팅이 가능한 'Midnight Lounge' 기능의 Node.js + WebSocket 서버 구조를 짤 거야. 위치 기반 인증(Geofencing) 로직을 처리하는 효율적인 방법과 방(Room) 관리 코드를 작성해 줘."

4. 마케팅 & 성장 전략 (Marketing Division)

⑦ 앱 스토어 옵티마이저 (App Store Optimizer)

프롬프트:

"Activate App Store Optimizer mode.
@seowl_context.md의 타겟 고객을 분석해서, 애플 앱스토어(App Store)와 구글 플레이(Google Play)에 올릴 Seowl의 앱 제목(Subtitle 포함), 10개의 핵심 검색 키워드, 그리고 유저의 다운로드를 유도하는 설득력 있는 긴 줄거리 설명문(Description)을 작성해 줘."

⑧ 레딧 커뮤니티 빌더 (Reddit Community Builder) / 그로스 해커 (Growth Hacker)

프롬프트:

"Activate Growth Hacker mode.
새벽 시간대 이용자(대리기사, 야간 작업자, 올빼미족)가 모여 있는 특정 온라인 커뮤니티(예: 블라인드, 디시인사이드, 오픈채팅방 등)에 초기 유저(CBT) 모집을 위한 게릴라 마케팅 게시글 초안을 작성해 줘. 대놓고 홍보하는 느낌이 아니라, 자연스럽게 '이런 불편함 없었어?'라고 공감대를 형성하는 방향으로 써야 해."

🚀 사용 팁 (Cursor/Windsurf 기준)

이 레포지토리의 에이전트들은 자신이 어떤 산출물(Deliverables)을 내야 하는지 명확히 알고 있습니다.
명령어를 치실 때 반드시 다음 3가지 요소를 포함하세요.

에이전트 소환: "Hey Claude (또는 에이전트명), activate [에이전트 이름] mode"

Seowl 컨텍스트 제공: "Read the @seowl_context.md to understand the product."

해당 에이전트 전용 미션 부여: 프론트 개발자에게 마케팅을 시키지 말고, 반드시 각각의 전문 분야에 맞는 작업을 명시해 주세요.

이렇게 사용하시면 혼자서도 기획자-디자이너-앱개발자-백엔드-마케터로 이루어진 풀스택 1인 개발사처럼 완벽하게 Seowl 프로젝트를 빌드해 나가실 수 있습니다.

Sources
help

github.com
medium.com
Google Search Suggestions
Display of Search Suggestions is required when using Grounding with Google Search. Learn more
"msitarzewski/agency-agents" github


+당근마켓 커뮤니티처럼 컨셉을 따라가면 좋을듯.
