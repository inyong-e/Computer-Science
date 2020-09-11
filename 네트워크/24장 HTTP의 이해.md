http method: 요청의 목적 : get ,post, put, head, delete

get: 리소스 요청 , post : 내용 전송 , put: 내용 갱신

head: 리소스에 대한 정보만 요청, delete : 리소스 제거

request target : 리소스 경로

### http Head

- accept : 클라이언트가 허용 가능한 파일 형식
- user-agent: 클라이언트의 os, 브라우저 정보
- host: 서버의 도메인 네임

### response

head+ body

version / status/ status message

### status code

200 : ok

307 : 리다이렉트

4xx : 클라이언트 문제, 잘못된 요청 (400: 잘못된 요청, 401: 권한 없음 404 : 없는 요청)

500 : 서버 내부 문제 발생

502: 게이트웨이 문제

503: 서버 가용 능력이 없음
