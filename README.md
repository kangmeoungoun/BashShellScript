### 리눅스 명령어
### 실무에서 자주 사용하는 명령어_I/O 관련 명령어
- I/O 관련 명령어
  - redirection : 표준 스트림(stdin,stdout,stderr) 을 부등호를 사용하여 지정한 위치로 보낼 수 있는 방향지정 옵션
  - echo : 문자열을 출력하는 도구
  
- User 관련 명령어
  - chmod(Change MODe) : 파일이나 디렉토리의 모든(접근권한) 을 변경하는 도구
  - chown(Change the OWNer of a file) : 파일의 소유권을 바꾸기 위한 도구
  - sudo (Superuser DO --> Substitude User DO) : root 사용자의 보안 권한을 이용하여 명령 또는 프로그램을 실행하는 도구
  - who : 현재 시스템에 로그인한 사용자 목록을 출력
```shell
echo a > a.txt  
> 매번 값 초기화
>> 기존 파일 내용 아래줄에 추가.
>| 쉘스크립트에서 사용 강제적으로 파일 생성 해준다 > 파일 없을때 에러난다.

유저 그룹 그외
rwx rwx rwx
421 421 421

chown 소유자며:그룹명 파일/디렉토리이름

w :who 상세정보

```