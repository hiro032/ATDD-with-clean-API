# ATDD-with-clean-API

##  MISSION 1. 인수 테스트
- 인수 테스트를 위한 환경 구축.
- 인수 테스트를 위한 도구 활용. (JUnit, AssertJ, RestAssured, JsonPath)
- clean API 설계.

### [GitHub 주소](https://github.com/next-step/atdd-subway-map/tree/hiro032)


|제목|내용|설명|
|------|---|---|
|[🚀 1단계 - 노선 관리 기능 구현](https://github.com/next-step/atdd-subway-map/pull/160)| 지하철 노선 관리 기능을 검증하는 인수 테스트 작성하기 </br>  인수 테스트로 도출된 시나리오를 충족하는 기능을 구현하기|지하철 노선 생성, 조회, 수정, 삭제기능을 검증하는 인수테스트 작성 |
|[🚀 2단계 - 인수 테스트 리팩터링](https://github.com/next-step/atdd-subway-map/pull/204)|새로운 기능을 추가하면서 인수테스트 리팩터링 하기| 지하철역과 지하철 노선 이름 중복 금지 요구사항 추가 </br> 추가된 요구사항을 구현하면서 인수 테스트 리팩터링 |
|[🚀 3단계 - 지하철 구간 관리](https://github.com/next-step/atdd-subway-map/pull/269)|새로운 요구사항을 통해 직접 인수 조건을 도출하고 인수 테스트 작성하기 |지하철 노선 생성 시 필요한 인자를 추가하기 구간 등록, 제거, 구간을 통한 역 목록 조회 기능 추가 |

---

##  MISSION 2. ATDD + TDD

### [GitHub 주소](https://github.com/next-step/atdd-subway-path/tree/hiro032)

- TDD와 인수 테스트를 함께 활용하기
- Inside Out TDD
- Outside In TDD
- 단위 테스트의 정의
- 통합 테스트의 정의
- 단위 테스트와 통합 테스트시 고려해야할 사항
- 스프링에서의 테스트 환경
- 테스트를 위한 도구 활용 ( JUnit, Mockito, JGraph)

|제목|내용|설명|
|------|---|---|
|[🚀 1단계 - 구간 추가 기능 변경](https://github.com/next-step/atdd-subway-path/pull/242)|변경된 스펙에 대한 인수 조건 도출 및 인수 테스트 작성</br> 비즈니스 로직 구현시 TDD로 구현| 역 사이에 새로운 역을 등록하는 기능 추가 </br> 변경된 요구사항에 맞게 인수 테스트를 수정하고 예외 케이스 까지 함께 인수 테스트 작성|
|[🚀 2단계 - 구간 제거 기능 변경](https://github.com/next-step/atdd-subway-path/pull/274)| 구간 삭제에 대한 제약 사항 변경 구현| 종점 제거시 다음으로 오던 역이 종덤이 됨. 구간이 하나인 노선에서 마지막 구간을 제거하는 경우와 같은 예외 상황도 고려|
|[🚀 3단계 - 경로 조회](https://github.com/next-step/atdd-subway-path/pull/276)| 최단 경로를 조회하는 요구사항 추가| 외부 라이브러리에 대한 테스트 작성, 중복된 데이터에 대한 픽스쳐 생성하기|

---

##  MISSION 3. ATDD 기반 리팩터링

### [GitHub 주소](https://github.com/next-step/atdd-subway-favorite/tree/hiro032)

- 인수 테스트에 대한 리팩터링
- 인수 테스트 통합
- 레거시 코드 리팩터링
- 인증과 인증 도구, 인증 프로세스 

|제목|내용|설명|
|---|---|---|
|[🚀 1단계 - 토큰 기반 로그인 구현](https://github.com/next-step/atdd-subway-favorite/pull/237)| JWT 토큰을 통한 로그인 기능 구현하기 | 스프링 인터셉터를 통해 권한이 필요한 요청시 사용자의 권한 확인 권한 확인 후 성공 후 처리 로직 구현|
|[🚀 2단계 - 인증 로직 리팩터링](https://github.com/next-step/atdd-subway-favorite/pull/243)| 기존 코드를 그대로 둔 채로 새로운 테스트 작성하기| 추상화를 통한 중복 로직 제거와 패키지간 양방향 의존성 제거하기|
|[🚀 3단계 - 즐겨찾기 기능 구현](https://github.com/next-step/atdd-subway-favorite/pull/247)| 새로운 요구사항인 즐겨찾기 기능 구현하기| 즐겨찾기 기능은 로그인을 한 사용자 한에서 가능하며 로그인하지 않은 사용자가 접근시 적절한 상태 코드로 응답 하기|

---

## MISSION 4. 테스트 기반 문서화

### [GitHub 주소](https://github.com/next-step/atdd-subway-fare/tree/hiro032)
- 스프링에서 다양한 테스트 환경 구축하기
- 문서 자동화 도구 학습하기 (Spring Rest Docs)


|제목|내용|설명|
|---|---|---|
|[🚀 1단계 - 경로 조회 타입 추가](https://github.com/next-step/atdd-subway-fare/pull/148)| 새로운 요구사항인 최소 시간 경로 타입 추가 기능 구현하기| 인수 시나리오를 도출하고 문서화 작업 이후 기능 구현하기|
|[🚀 2단계 - 요금 조회](https://github.com/next-step/atdd-subway-fare/pull/149)| 요금 조회 기능 구현하기| 기본 운임 비용과 리 초과시 추가 운임 비용 계산하기|
