### 리눅스 명령어
### 실무에서 자주 사용하는 명령어_프로세스관련_명령어
- 프로세스 관련 명령어
    - top : 프로세스 목록을 일정 시간마다 새로고침하여 화면에 출력하는 툴 시스템 전반적인 상황을 모니터링 할 수 있음
      - top 한상태에서 1누르면 cpu 코어별로 용량 k누르면 kill 할수 있다.
    - nohup(NO HangUPs) : 쉘 스크립트 파일을 데몬 형태로 실행 표준 출력을 지정한 파일로 리다이렉트
    - kill : 지정한 프로세스에 지정한 시그널을 보내 프로세스 종료
  
```shell
nohup echo "Bash Commnad"
[root@67c211f24ca1 work]# cat nohup.out
Bash Commnad

INT TERM 프로세스를 안전하게 종료 전부작업처리후 종료

kill -2 프로세스번호 
kill -INT 프로세스번호

kill -15 프로세스번호
kill -TERM 프로세스번호

kill -9 프로세스번호
kill -KILL 프로세스번호

좀비 프로세스는 2 15 로 죽지 않는다.
```