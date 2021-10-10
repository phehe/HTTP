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
  6. Start-line -> GET/POST/PUT 등 
  7. Header
  8. Empty line
  9. Message Body
  10. 단순, 확장 가등
