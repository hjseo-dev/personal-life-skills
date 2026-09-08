# personal-life-skills

개인/생활용 Claude Code 스킬 모음. `life` 플러그인 하나에 스킬들이 모여
있고, 각 스킬은 `/life:<스킬명>`으로 호출한다.

원래 [study_claude](https://github.com/hjseo-dev/study_claude) 저장소의
`wlabs` 플러그인에서 개인/생활용 스킬만 분리해 나온 저장소다.

## 스킬 목록 (서로 독립 — description의 경계 문구로만 구분)

| 스킬 | 하는 일 | 헷갈릴 수 있는 이웃 |
|---|---|---|
| `weather` | 독산1동 기준 오늘 날씨 조회 | `umbrella`와 API 공유, 목적으로 구분 |
| `umbrella` | 독산1동 기준 1~2시간 내 우산 필요 여부 | `weather` 참고 |
| `home-eta` | 자취방→본가 출발시점별 소요시간(Tmap) | `drive-cost`와 "고정 구간·ETA" vs "임의 구간·비용"으로 구분 |
| `drive-cost` | 임의 구간 왕복 톨비+기름값 계산 | `home-eta` 참고 |
| `cafe-with-study` | 지역 기반 "공부하기 좋은 카페" 추천 | — |
| `jeju-trip-plan` | 제주 숙소 근처 날짜별 여행 일정 생성 | — |
| `bookmark` | URL 내용을 정리해 로컬 마크다운으로 저장 | — |
| `fconline` | FC온라인 최근 전적 분석 + 전술 추천 | — |
| `stock-picks` | 관심 테마별 시가총액 top3 조회 | `stock-screener`와 "순위만" vs "심층분석"으로 구분 |
| `stock-screener` | 개별 종목 재무제표(ROE·부채비율 등) + 밸류에이션(PER·PBR·PEG) 분석 | `stock-picks` 참고 |
| `savings-compare` | 실제 예금/적금 상품 API 비교, 세후 수령액 최고 상품 추천 | `goal-saving-planner`와 "실제 상품" vs "가정 기반 시뮬레이션"으로 구분 |
| `goal-saving-planner` | 월급/고정비 기반 카드값 한도 역산 + 30년 복리 자산 시뮬레이션 | `savings-compare` 참고 |
