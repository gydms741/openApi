# RestAPI

## REST 특징
- Representational State Transfer
- REST는 네트워크 상에서 Client와 Server사이의 통신 방식 중 하나이다.
- REST는 기본적으로 웹의 기존 기술과 HTTP 프로토콜을 그대로 활용하기 때문에 웹의 장점을 최대한 활용할 수 있는 아키텍처 스타일이다.

### 1. Server-Client(서버-클라이언트 구조)
- 자원이 있는 쪽이 Server, 자원을 요청하는 쪽이 Client가 된다.
- REST Server : API를 제공하고 비즈니스 로직 처리 및 저장을 책임진다.
- Client : 사용자 인증이나 context(세션, 로그인 정보) 등을 직접  관리하고 책임진다.
- 서로 간 의존성이 줄어든다.

### 2. Stateless(무상태)
- HTTP 프로토콜은 Stateless Protocol이므로 Rest역시 무상태성을 갖는다.
- Client의 context를 Server에 저장하지 않는다. 즉, 세션과 쿠키와 같은 context정보를 신경쓰지 않아도 되므로 구현이 단순해진다.
- Server는 각각의 요청을 완전히 별개의 것으로 인식하고 처리한다.
- 각 API서버는 Client의 요청만을 단순 처리한다.

### 3. Cacheable(캐시 처리 가능)
- 웹 표준 HTTP 프로토콜을 그대로 사용하므로 웹에서 사용하는 기존의 인프라를 그대로 활용할 수 있다.
- 대량의 요청을 효율적으로 처리하기 위해 캐시가 요구된다.
- 캐시 사용을 통해 응답시간이 빨라지고 REST Server 트랜잭션이 발생하지 않기 때문에 전체 응답시간, 성능, 서버의 자원 이용률을 향상시킬 수 있다.

### 4. Layered System(계층화)
- Client는 REST API Server만 호출한다.
- REST Server는 다중 계층으로 구성될 수 있다.
- PROXY, Gateway 같은 네트워크 기반의 중간 매체를 사용할 수 있다.

### 5. Code-On-Demand(Optional)
- Server로부터 스크립트를 받아서 Client에서 실행한다.

### 6. Uniform Interface(인터페이스 일관성)
- URI로 지정한 Resource에 대한 조작을 통일되고 한정적인 인터페이스로 수행한다.
- HTTP 표준 프로토콜에 따르는 모든 플랫폼에서 사용이 가능하다.

---

## API란
- API는 애플리케이션 소프트웨어를 구축하고 통합하기 위한 정의 및 프로토콜 세트로, Application Programming Interface를 나타낸다.
- 데이터와 기능의 집합을 제공하여 컴퓨터 프로그램간 상호작용을 촉진하며, 서로 정보를 교환 가능 하도록 하는 것

---

## REST API란

- REST API의 정의

REST기반으로 서비스 API를 구현한 것.

최근 Open API, 마이크로 서비스를  제공하는 업체 대부분은 rest api를 제공한다.
