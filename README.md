### 리눅스 명령어
### 실무에서 자주 사용하는 명령어_네트워크 관련 명령어
- 네트워크 관련 명령어
  - iptables : 패킷 필터링 도구로 패킷의 출입을 제한하는 방화벽구성이나 NAT(Network Address Translation)구성에 사용
  - ufw(Uncomplicated FireWall) : iptables의 제어를 쉽게 하기 위한 도구
  - ping : ICMP 프로토콜의 응답 확인 도구
```shell
iptables -nL 
들어오는 통신을 다 막고 필요한 것만 여는 방식 기본 정책.

ping -c 5  localhost 5번만 보내고 종료 
```