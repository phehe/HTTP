# HTTP

### IP

  1. Packet -> 출발, 도착IP/Data
  2. 비연결성, 비신뢰성
    
### TCP

  1. 출발,도착 IP + 출발, 도착 PORT + 전송제어, 순서, 검증
  2. TCP 3 way handshake(SYN/SYN,ACK/ACK->Data 전송)
  3. Data 전달 보증, 순서 보장 -> 신뢰할 수 있는 프로토콜


### UDP

  1. 무색 -> 연결지향, 데이터 전달 보증, 순서 보장 XXXXX
  2. 단순하고 빠르다
  3. IP와 비슷 + PORT


### URI/URL

  1. host:port/path[?query]  -> 식별/위치
  
### HTTP

  1. HTTP 1.1 / 2 / 3 
  2. Client ---- Server 구조  --> (Request ---- Response)
  3. Stateless ---- Stateful  --> Stateless(서버가 클라이언트의 상태를 보존 XXX -> 서버 확장성 높음(스케일 아웃)
  4. HTTP 메시지
  5.    SHEM ->
  6. Start-line -> GET/POST/PUT/DELETE 등 
  7. Header     -> 표현데이터 
  8. Empty line -> 그냥 빈 줄
  9. Message Body-> 메세지
  10. 단순, 확장 가등

### HTTP Method
  API
  1. URI -> 리소스를 식별하는게 가장 중요    ex) members -> 회원 자체의 식별 -> 부가적인 부분은 HTTP 메서드가 처리한다.
  @ CRUD ===== PGPD
  @ POST => Client -> Server에 요청하면 서버가 메시지로 들어온 데이터 처리  -> 신규 리소스 생성
  @ GET  => Client -> Server에 전달하고 싶은 데이터 -> 쿼리파라미터, 쿼리스트링을 통해서 전달 (ex) -> /search?q=hello&hi=KO) -> 리소스 조회
  @ PUT  => 리소스가 존재하면 대체, 없으면 생성 -> 덮어쓰기 생각  -> Client가 리소스를 식별한다. 
 
  #### HTTP METHOD 속성
    1. 안전, 멱등, 캐시가능  
    @ 안전 -> 호출해도 리소스 변경 X
    @ 멱등 -> 한 번 호출, 여러번 호출 -> 결과는 똑같다  -> POST만 아니다 (결제 시스템 생각)
    @ 캐시가능 -> 응답 결과 리소스를 캐시해서 사용 -> GET, HEAD
    
### HTTP State Code
  1. 1xx 처리중
  2. 2xx 요청 성공 -> 200 (OK), 201(요청 성공 -> 새로운 리소스 생성)
  3. 3XX 요청 완료하기 위해 추가 작업 필요 -> 301(요청메서드 GET or 본문 제거), 308(요청 데이터 유지)
                                         -> 302(리다이렉트 요청시 메서드가 GET으로 변하고 본문이 제거)
                                          -> 304(캐시 목적 사용 -> 로컬 PC에 저장된 캐시 재사용)
  4. 4XX Client 문제 -> Server가 요청 수행할 수 없음.
  5. 5XX Server 내부 문제                                          
  
  





