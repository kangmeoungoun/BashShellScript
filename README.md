### 리눅스 명령어
### 실무에서 자주 사용하는 명령어_디렉토리와 파일 통계
- 파일 시스템 관련 명령어
  - mkdir(Make Deirectory) : 디렉토리를 생성
  - rmdir(Remove Directory) : 디렉토리를 삭제
  - pwd(Print Working Driectory) : 현재 위치한 디렉토리의 절대경로를 출력
  - mount : 디스크 장치를 표시하거나 가상 파일 시스템으로 지정한 디렉토리를 연결
     ex) PC 방 옆자리컴퓨터에  공유폴더를 만들어서 내자리에서 탐색기에서 공유폴더 접근
  - stat : 지정한 파일의 파일통계를 출력

```shell
mount -t nfs ip주소:/nfs /mnt      
/nfs 상대방 디렉토리
/mnt 로컬디렉토리
```
