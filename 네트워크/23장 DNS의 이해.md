# DNS

호스트(도메인) 이름을 Ip 주소로 변환 - port 53

![image](https://user-images.githubusercontent.com/13481627/92919386-58665180-f46b-11ea-8376-dfd9318491f3.png)

### 쿼리 과정

![image](https://user-images.githubusercontent.com/13481627/92919542-a67b5500-f46b-11ea-9275-716838b2301e.png)

### Records 타입

- A: 호스트 명
- NS: 네임 서버
- CNAME: 별칭
- MX: 메일 서버

### Hosts.txt

호스트 이름과 IP 주소가 맵핑되어 저장된 파일
Local DNS로 쿼리 전에 우선 참조 하는 파일

### DNS 캐시 테이블

기존에 응답 받은 DNS 정보를 일정시간 저장하고 동일한 질의 시 응답

### DNS 동작 과정

1. PC에서 웝 사이트 접속한다
2. DNS에 www.daum.net이 뭔지 물어보면 DNS가 해당 아이피를 알려준다.

3. PC 네트워크 환경 확인 - primary DNS 8.8.8.8(구글 네임 서버)로 설정되어있음.
4. hosts.txt 파일 참조 - 해당 도메인이 설정된 경우 맵핑된 IP 로 응답
5. dns cache table 참조 - 해당 도메인이 저장된 경우 저장된 iP로 바로 응답

6. 둘다 없으면 local DNS(8.8.8.8)에게 쿼리
