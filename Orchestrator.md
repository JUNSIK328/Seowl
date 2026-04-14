# 🦉 Seowl (서울): 마스터 워크스페이스 & 오케스트레이션 가이드

**프로젝트 명칭:** Seowl (Seoul + Owl)
**비전:** "잠들지 않는 서울을 즐기는 모든 이를 위한 심야 특화 라이프스타일 SNS & 지도"
**슬로건:** Seoul never sleeps, and neither does Seowl.

---

## 📖[Part 1] 프로젝트 핵심 정의 (Project Context)

### 1. 코어 타겟 (Target Audience)
*   **🚗 Drive-Owls:** 심야 드라이브, 뷰, 야간 주차 니즈.
*   **🛴 Active-Owls:** 막차 끊긴 후 N버스, 킥보드, 따릉이 이용 객.
*   **💻 Work-Owls:** 심야 노트북 작업 (콘센트, 와이파이, 백색소음 중시).
*   **🛡️ Safe-Owls:** 막차 이후 안심할 수 있는 24시 대기 거점 (편의점 등).

### 2. 핵심 무기 (Key Features & Moat)
*   **뱀파이어 모드 UI:** 다크모드 베이스. 빛 공해 최소화 및 야간 감성 자극.
*   **Proof of Life (실시간 생존 신고):** 네이버 지도의 부정확한 24시간 정보 대신, 유저 위치 기반(GPS) 실시간 "여기 문 열었음" 체크인 연동.
*   **Owl-Eye Filter:** 심야 치안 안심지수, 콘센트 위치, 야간 작업/드라이브 난이도 필터.
*   **Midnight Lounge:** 반경 1km 기반의 1회성/시간 한정(자정~새벽 4시) 위치기반 채팅방.

---

## 🚀 [Part 2] 12단계 실무 파이프라인 (Agency-Agents 지정 목록)
**총괄 `Agents Orchestrator`는 아래 명시된 담당 에이전트(Assigned Agent)를 순서대로 호출할 것.**

###[Phase 1: 기획 및 UI 빌드 (App Foundation)]
1. **[구조 설계] `UX Architect`:** Seowl 앱 최초 실행 시 [Drive / Active / Work / Safe] 올빼미 유형을 선택하는 3단계 온보딩 플로우 와이어프레임 텍스트 구성.
2. **[디자인/무드] `UI Designer`:** 뱀파이어 모드 테마에 맞는 메인 컬러(HEX) 코드 및 텍스트 대비(Contrast) 시스템 제안.
3. **[게이미피케이션] `Whimsy Injector`:** Proof of Life 체크인 성공 시 유저에게 재미(도파민)를 줄 수 있는 매이크로 카피(문구)와 애니메이션 기획.
4. **[모바일 앱 구축] `Mobile App Builder`:** React Native 베이스의 지도 렌더링 프레임, 하단 토글(뚜벅이/운전 모드) 레이아웃 코드 작성.

###[Phase 2: 백엔드 및 인프라 구축 (System & Cloud)]
5. **[DB 아키텍처] `Backend Architect`:** 밤 시간대 트래픽 쏠림과 위치 기반(반경 2km 이내 검색) 매칭을 감당할 Node.js + PostGIS + Redis 구조도 및 샘플 쿼리 설계.
6. **[서버 스케일링] `DevOps Automator`:** 자정부터 새벽 4시에 서버를 증설하고, 아침 8시에는 최소한으로 축소하는 AWS 클라우드/서버리스 환경 구축 파이프라인 제시.

###[Phase 3: 무결성 검증 (Security & QA)]
7. **[치안 및 정책] `Brand Guardian` & `Legal Compliance`:** (협업) 심야 커뮤니티 채팅방 내에서 어뷰징(조건만남 등) 방지를 위한 커뮤니티 규칙 설계 및 [위치기반 서비스 이용약관] 필수조항 검토.
8. **[어뷰징 공격 테스트] `Reality Checker` & `API Tester`:** 유저가 GPS를 스푸핑(조작)하여 가짜 체크인을 할 경우를 가정하여 시스템 방어 로직 설계.

###[Phase 4: 마케팅, GTM 전략 및 투자 유치 (Growth)]
9. **[유저 확보 - 숏폼] `TikTok Strategist`:** "네이버지도 '영업 중' 마크에 속아 밤길 헛걸음"한 경험을 살린 15초 B급 감성 바이럴 영상 대본 제작.
10. **[게릴라 초기 침투] `Reddit Community Builder`:** 밤 시간대 올빼미/개발자/드라이버 들이 서식하는 커뮤니티(에브리타임, 보배드림, 블라인드) 잠입 홍보 문구 기획.
11. **[스토어 등록] `App Store Optimizer`:** 밤드라이브, 24시카페 등 ASO(앱스토어 검색 최적화) 기반 앱 제목/키워드 배열 최적화.
12. **[IR 피치덱 생성] `Exec Summary Gen.`:** 엔젤 투자 심사역을 설득하기 위한 엘리베이터 피치 작성 및 사업계획서/Pitch Deck 목차 10p 초안 요약 작성.

---

## 🎛️ [Part 3] 시스템 가동 프롬프트 

```text
Activate `Agents Orchestrator` mode. 

우리는 "Seowl"이라는 올빼미족을 위한 심야 특화 앱을 개발하고 런칭할 거야. 
현재 디렉토리에 있는[Part 1] 및 [Part 2] 내용을 기반으로 프로젝트의 총괄 오케스트라 지휘자가 되어 줘.

**진행 방식 가이드:**
너는 내가 지정한 **[Phase 1 ~ Phase 4] (총 12단계) 리스트**를 차례대로 하나씩만 처리해 나간다. 
임의로 에이전트 이름을 만들지 말고, `agency-agents` 리스트에 존재하는 **명시된 에이전트 이름 그대로 호출**하여 롤플레이(Roleplay)를 전환한 뒤 결과물을 뽑아줘.

지금 당장 Phase 1의 첫 번째 과제인 **`UX Architect`**를 소환해서 앱 온보딩 텍스트 구조 설계 결과를 먼저 출력해라. 그리고 나(유저)의 검토와 지시를 기다려라.
