### 리눅스 명령어
### 실무에서 자주 사용하는 명령어_네트워크 관련 명령어
- 네트워크 관련 명령어
    - ifconfig(Interface CONFIGuration) : 네트워크 인터페이스의 활성/비활성화 및 설정
    - ip : ip 관련 정보 조회 및 설정
    - netstat (NETwork STATistics) : 네트워크 프로토콜의 통계와 연결상태를 출력
    - ss(SOcket Statistics) : 네트워크 소켓의 통계와 연결상태를 출력
```shell
ip address show

네트워크 관련정보
ls -al /etc/sysconfig/network-scripts/

netstat -nltpu (n:도메인이름이나 포트를 숫자로 표현,l:리스닝 을 하고 있는 상태,t:tcp통신,p:프로그램이름,u:udp통신)
netstat -tanu 현재네트워크 상태 전체 

약속된 해당 port 출력
cat -n /etc/services

```    