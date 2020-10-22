# RESTful API

### RESTful API란?

- REST ( REpresentational State Transfer)  

  자원을 이름(자원의 표현)으로 구분하여 해당 자원의 상태(정보)를 주고 받는 모든 것을 의미한다

- API(Application Programing Interface)

  어떠한 응용프로그램에서 데이터를 주고 받기 위한 방법을 의미

- RESTful API

  REST의 기본 원칙을 성실히 지킨 API

### REST 6가지 원칙

1. Uniform Interface

   URI로 지정한 리소스에 대한 조작을 통일되고 한정적인 인터페이스로 수행

2. Stateless

   작업을 위한 상태정보를 따로 저장하고 관리하지 않음

3. Cacheable

   HTTP 기존 웹 표준 그대로 사용하여 웹에서 사용하는 기존 인프라 그대로 활용 가능

4. Self-descriptiveness

   REST API 메세지만 보고도 이를 쉽게 이해 할 수 있는 자체 표현 구조로 되어있음

5. Client-Server 구조

   REST 서버는 API 제공, 클라이언트는 사용자 인증이나 컨텍스트(세션,로그인 정보)등을 직접 관리

6. 계층형 구조

   REST 서버는 다중 계층으로 구성될 수 있다.

### RESTful 하게 API를 디자인 한다는 것은 무엇을 의미하는가?

1. 리소스와 행위를 명시적이고 직관적으로 분리한다
   - 리소스는 URI로 표현되는데 리소스가 가리키는 것은 명사로 표현
   - 행위는 HTTP Method로 표현, get , post , put , patch , delete을 분명한 목적으로 사용
2. Message는 Header와 Body를 명확하게 분리해서 사용
3. API 버전을 관리
4. 서버와 클라이언트가 같은 방식을 사용해서 요청하도록 한다
   - 브라우저는 form-data 형식의 submit 으로 보내고 서버에서는 json 형태로 보내는 식의 분리보다는 json 으로 보내든, 둘 다 form-data 형식으로 보내든 하나로 통일한다.

### 어떠한 장점이 존재하는가?

1. Open API를 제공하기 쉽다.
2. 멀티플랫폼 지원 및 연동이 용이
3. 원하는 타입으로 데이터를 주고 받을 수 있다.
4. 기존의 웹 인프라(HTTP)를 그대로 사용할 수 있다.

### 단점

1. 사용할 수 있는 메소드가 4가지 밖에 없다.
2. 분산환경에는 부적합
3. HTTP 통신 모델에 대해서만 지원

