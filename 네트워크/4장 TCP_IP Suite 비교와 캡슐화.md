# TCP/IP 정의

네트워크 프로토콜의 모음으로 '패킷 통신 방식'의 IP와 '전송 조절 프로토콜'인 TCP로 이루어져 있다

## TCP/IP 모델

### Network interface 계층

물리계층으로 네트워크 노드들을 상호 연결

### Network 계층

패킷을 처리하고 다른 네트워크로 연결

### Transport

TCP / UDP

### Application

응용 프로그램간 표준화 된 데이터 교환

# 캡슐화

모든 네트워크는 캡슐화하여 통신한다.

### 인캡슐레이션

하나하나씩 캡슐화 시킴

- Application 계층에서 Host Data (사람이 캐릭터나 그림을 보내는 등 데이터 전송)
- presentation에서 session에서 이해할 수 있는 정형화된 Data로 캡슐화
- session에서 Data 캡슐화 ()
- Transport 에서 Data + TCP header(어떤 포트를 사용할 건지) (데이터가 segment)
- Network에서 Data + IP header(어떤 IP 목적지인지) (packet)
- DataLink에서 Data + Mac address(어떤 컴퓨터인지) Header
- physical에서 signal 11011011011010101 방식으로 전송

### 디캡슐레이션

반대로
