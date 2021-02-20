### 리눅스 명령어
### 실무에서 자주 사용하는 명령어_디렉토리와 파일 통계
- 파일 시스템 관련 명령어
  - cd(Change Directory) : 현재 작업 디렉토리를 지정한 디렉토리로 변경
    - cd - : 바로 직전의 있던 위치로 이동
  - ls(List) : 현 디렉토리의 파일 목록을 출력
    - ls 옵션 : 1(파일명세로정렬) h(용량 보기편하게) t(시간순서order by) r(역순)
  - df(Disk Free) : 마운트된 모든 장치에 대한 현재의 디스크 공간 통계를 출력
  
- 절대경로 : 최상위 디렉토리에서 지정한 디렉토리 까지 가는 길
- 상대경로 : 현재위치에서 지정한 디렉토리 까지 가는 길

```shell
ls -al | awk '{print $9}'
```
