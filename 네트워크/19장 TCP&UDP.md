# Transport 계층

end to end 서비스, 커넥션을 관리 . 1:1 커넥션 관리

### port

전송 계층에서 사용되며 특정 프로세스를 구분하는 단위

### TCP

전송 제어 프로토콜

인터넷을 구성하는 핵심 프로토콜

신뢰성을 기반으로 데이터를 에러 없이 전송, 1:1 통신

에러 발생시 재전송을 요청하고 에러를 복구한다.

```
segment -> TCP header + Data (TCP header에는 소스 포트와 목적지 포트,회선 제어 관리 플래그, 흐름 제어 정보, 데이터 무결성 확인 등 통신 제어에 필요로 여러가지 정보가 들어있음 )

네트워크 계층의 packet => IP header + segment
```

![image](https://user-images.githubusercontent.com/13481627/92844672-13b5c880-f421-11ea-95bf-88a32dea2eb7.png)

### UDP

신뢰성은 낮으나 데이터 전송이 빠르다,

송신측은 일반적으로 데이터를 보내고 확인 안함. 1:n 통신 가능

실시간 데이터 전송에 적합

스트리밍 서비스의 경우 전송 문제가 발생해도 재전송 보다는 실시간 데이터 전송이 중요

segment -> UDP header + Data (TCP header에는 소스 포트와 목적지 포트, 전체 데이터 길이, 데이터 무결성)

네트워크 계층의 packet => IP header + segment
