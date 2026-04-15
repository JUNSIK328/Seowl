
```markdown
# 🦉 Seowl

**Seoul never sleeps, and neither does Seowl.**

잠들지 않는 서울을 위한 **심야 특화 라이프스타일 지도 + SNS**  
운전자·뚜벅이·작업자·안전 올빼미 모두를 위한 밤의 생존 키트.

---

## 🎯 Seowl이 만드는 것

### 핵심 타겟
- **Drive-Owls** — 심야 드라이브족 (주차·방지턱 제로 루트·세차)
- **Active-Owls** — N버스·킥보드·따릉이족
- **Work-Owls** — 새벽 작업자 (콘센트·백색소음·24시 카페)
- **Safe-Owls** — 막차 놓친 안전 올빼미

### 진짜 차별점 (네이버지도와의 Moat)
- **뱀파이어 모드** — 눈 피로 ZERO 네이티브 다크모드 + 스텔스 UI
- **Proof of Life** — 유저 실시간 “지금 영업 중” GPS 체크인 (가짜 24시 표기 퇴치)
- **Owl-Eye Filter** — 안심지수, 콘센트, CCTV, 마감임박 할인 등 밤에만 의미 있는 필터
- **Midnight Lounge** — 특정 핫스팟 반경 1km 안에서만 열리는 위치 기반 실시간 채팅

---

## 📁 파일 구조 (현재 정리 완료)

```
Seowl/
├── README.md
├── docs/                  ← 모든 기획 문서 모음
│   ├── seowl_master_workspace.md   ← ★ 진짜 핵심 마스터플랜
│   ├── masterplan.md
│   ├── Orchestrator.md
│   ├── inst.md
│   ├── newidea.md
│   └── report.md
├── prompts/               ← (추후) 에이전트별 프롬프트 모음
└── src/                   ← (개발 시작 후) 실제 코드
```

**가장 중요한 파일**  
→ `docs/seowl_master_workspace.md` (프로젝트 전체 컨텍스트 + 11단계 파이프라인)

---

## 🚀 이 레포의 진짜 목적

**혼자서도 11명의 전문가 팀을 데리고 풀스택 개발하는 설명서**

Cursor, Claude, Windsurf 등 AI 에이전트(Agency-Agents)를 활용해  
기획 → 디자인 → 프론트 → 백엔드 → 마케팅까지 **릴레이**로 만들어가는 워크플로우 가이드입니다.

### 사용 방법 (초간단 3단계)

1. `docs/seowl_master_workspace.md`를 `@seowl_context.md`로 복사해서 최상위에 두기 (에이전트들이 읽기 쉽게)
2. Orchestrator를 먼저 깨우기 (아래 프롬프트 복붙)
3. Phase 1 Step 1부터 하나씩 진행 (승인받고 다음 단계로)

---

## 🧩 11단계 멀티-에이전트 파이프라인 (Masterplan 기준)

**Phase 1** — MVP 뼈대 만들기
1. Product Manager
2. UI Designer
3. Frontend Developer
4. Backend Architect
5. Growth Hacker
6. Data Researcher

**Phase 2** — 스케일업 & 방어
7. Red Teamer (보안)
8. DevOps
9. Legal Advisor
10. ASO Expert
11. Venture Capitalist (IR)

---

## 🔥 바로 시작하고 싶다면?

**Orchestrator 깨우기 프롬프트** (복사해서 바로 붙여넣기)

```markdown
Activate Orchestrator mode.

@docs/seowl_master_workspace.md 전체를 읽고 이해했어.
우리는 11단계 파이프라인을 따라 Seowl을 만들 거야.

지금 당장 **Phase 1 - Step 1: Product Manager**부터 시작해.
초기 온보딩 화면 설계 + 심야 익명 라운지 커뮤니티 가이드라인 5가지를 만들어서 보고해.
```

---

**추가로 미친 아이디어들은 `docs/newidea.md`에 잔뜩 있음**  
(뱀파이어 모드, 야광 포스터, 올빼미 계급제, 심야 세차 번개 등)

---

**준비됐으면 말해.**

“Orchestrator 지금 깨워” 라고 하면  
바로 Step 1 결과물 만들어줄게.

Seowl, 같이 밤새 만들어 보자 🔥
```

---

이 내용으로 교체하면  
- 현재 모든 md 파일 내용이 잘 녹아들어가고  
- 파일 구조 정리한 것도 반영됐고  
- GitHub에서 바로 예쁘게 보임

바로 교체할까? 아니면 조금 더 수정 원하는 부분 있어? (예: 더 짧게, 더 길게, 영문 버전 추가 등)
