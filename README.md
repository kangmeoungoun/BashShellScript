### 리눅스 명령어
### 실무에서 자주 사용하는 명령어_네트워크 관련 명령어
- 네트워크 관련 명령어
  - wget (Worl wide web + GET) : 웹서버로부터 컨텐츠를 가져오는 도구(프로그램의 설치파일을 다운로드 받을떄 사용.)
  - curl (Client for URLs) : 다양한 프로토콜을 사용하여 데이터를 전송하게 해 주는 도구
  - route : 네트워크의 경로 정보(라우팅 테이블)의 출력, 변경하는 도구
  

```shell
wget https://openresty.org/download/openresty-1.19.3.1.tar.gz 

curl -Lkso /dev/null -w "%{http_code}\n" https://gmail.com 
L :리다이렉트 링크를 따라 가는것.
k : https 인증을 무시해라
s : 통계갑 출력 무시 silent
o : output 파일 지정
/dev/null : 장치파일 아무것도 없는것. 중요
w : oupformat 결정.
l
```