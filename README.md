### 리눅스와 쉘
### 리눅스와 쉘(Bash)
- 유용한 Bash 커맨드라인 단축키
  - Tab : 명령 자동완성
  - Ctrl + c: 인터럽트 시그널을 보내 실행 중인 프로세스를 중단
  - Ctrl + a: 라인 맨 앞으로 커서 이동
  - Ctrl + e: 라인 맨뒤로 커서 이동
  - Ctrl + r: history 검색
    - Ctrl + r 입력후 검색어 입력 한디 다시 Ctrl + r 누르면 뒤에계속 찾아준다. 

```shell
cd : ChangeDirectory
pwd : printWorkingDirectory
//1씩 증가하면서 1초마다 print 
num=0; while true;do ((num+=1)); echo ${num}; sleep 1;done
```
