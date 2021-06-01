### `스프링 부트`와 `스프링 클라우드`로 구축한 `마이크로서비스 셋` 프로젝트

#### `API`와 `메시지` 기반의 `비동기` 서비스를 모두 지원하는 `리액티브` 마이크로서비스를 만들었습니다.

### 소개 

`스프링 웹플럭스` 및 `스프링 폭스`로 문서화가 잘 된 API를 만들었고, 
`스프링 데이터` `MongoDB`와 `JPA`를 사용해 `MongoDB`와 `SQL 데이터베이스`에 데이터를 저장했습니다.
`RabbitMQ`, `카프카`, `도커`, `스프링 클라우드 스트림`을 사용하여 비동기 서비스를 구축했고,
`프로젝트 리액터` 기반의 `논블로킹 API`와 `이벤트 기반 비동기 서비스`를 사용하여 `리액티브 마이크로서비스`를 구축하였습니다.
또한, 마이크로서비스와 데이터베이스, `메시징 시스템`으로 구성된 시스템 환경을 구축하고 테스트 하였습니다.
`스프링 클라우드`를 사용하여 확장성, 견고성, 보안성, 탄력성과 구성 가능성이 있고 상용화 준비가 완료된 서비스를 구축하였습니다.


### 구성

- `스프링 빈`을 기반으로 하는 비지니스 로직 구현
- `스프링 웹플럭스`를 기반으로 하는 REST API 구현 (`논블록킹` `동기` REST API 포함)
- `스프링 클라우드 스트림`을 사용한 `메시지` 기반의 `비동기` 서비스 구현 
- `스프링 폭스`와 `스웨거`/`OpenAPI`를 사용한 REST API 문서화
- `스프링 데이터`를 사용한 SQL/NoSQL 데이터베이스 구축
- `RabbitMQ`, `카프카`, `도커`, `스프링 클라우드 스트림`을 사용한 비동기 서비스 구축
- `프로젝트 리액터` 기반의 `논블로킹 API`
- `이벤트 기반 비동기 서비스`를 사용하여 `리액티브 마이크로서비스` 구축
- `마이크로서비스`와 `데이터베이스`, `메시징 시스템`으로 구성된 시스템 환경 구축
- `스프링 클라우드`를 사용하여 `서비스 검색`, `에지 서버`, `구성 중앙화`, `서킷 브레이커`, `분산 추적` 적용

### 사용한 기술

- `스프링 부트`
- `스프링 웹플럭스`
- `스프링 폭스`
- `스프링 데이터`
- `스프링 클라우드 스트림`
- `도커`
- `RabbitMQ`
- `카프카`
- `프로젝트 리액터`
- `스프링 클라우드`
   - 넷플릭스 `유레카`(검색 서버)
   - 넷플릭스 `리본`(클라이언트 측 로드 밸런서)
   - 넷플릭스 `주울`(에지 서버)
   - 넷플릭스 `히스트릭스`(서킷 브레이커)

### 개발 환경을 위한 필요 도구

- `Git`
- `Java`
- `curl`
- `jq`
- `Spring Boot CLI`

### 사용한 개발 도구
- `MapStruct` 자바 빈 매핑 도구, 스프링 데이터 엔티티 객체와 API 모델 클래스 상호 변환

### 마이크로서비스 구조

- 마이크로서비스 구조

<img src="resources/images/Microservice.png" title="구조"></img><br/>

- 영속성 추가

<img src="resources/images/Persistence.png" title="영속성 추가"></img><br/>

- 논블로킹 동기 REST API

<img src="resources/images/Nonblocking_API.png" title="논블로킹 동기 REST API"></img><br/>