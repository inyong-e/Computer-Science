### AS : 하나의 관리자 집단이 관리할 수 있는 네트워크 영역, 그룹

## EGP

외부 목적지로 가기 위해 어느 게이트웨이로 보내야 하는지 찾는 라우팅 프로토콜

### BGP

현재 인터넷에서 쓰이는 가장 대표적인 EGP 라우팅 프로토콜

ISP to ISP 연결 간 사용

경로 벡터 라우팅 프로토콜을 사용 - 루핑 방지

유니캐스트로 라우팅 정보전송

빠른 속도 보다는 조직 또는 단체 간 맺어진 정책에 의거하여 최적 경로 결정

## IGP

내부에서 어느 목적지로 가야 하는지 찾는 라우팅 프로토콜

### RIP

DIstance Vector 기반의 IGP용 라우팅 프로토콜

속도가 아닌 거리 기반 경로 선택
구성 간단, 적은 메모리, 소규모 네트워크에서 주로 사용

### OSPF

RIP 방식을 보완한 프로토콜
Link state 기반.

대규모 시스템에 적합.
