### 리눅스 명령어
### 실무에서 자주 사용하는 명령어_프로세스관련_명령어
- 프로세스 관련 명령어
    - ps(Process Status) : 시스템에서 실행중인 프로세스에 대한 정보를 출력
    - pstree(Process Status TREE) : 시스템에서 실행 중인 프로세스에 대한 정보를 트리구조로 출력
    - top : 프로세스 목록을 일정 시간마다 새로고침하여 화면에 출력하는 툴 시스템 전반적인 상황을 모니터링 할 수 있음

```shell
ps -ef 
ps aux :메모리 사용량 등 보여준다.
ps axfwwwww : 뒤에 명령어 짤린것들도 다 보여준다.

yum -y install psmisc
pstree
```    