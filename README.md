### 리눅스 명령어
### 실무에서 자주 사용하는 명령어_파일관련_명령어
- 파일 시스템 관련 명령어
  - cp(Copy) : 지정한 파일을 지정한 위치와 이림으로 복사
  - mv(Move) : 지정한 파일을 지정한 위치와 이름으로 이동
  - rename : 지정한 규칙에 따라 여러 개의 파일 이름을 변경
  - rm(Remove) : 지정한 파일을 삭제
  - less : 상하로 커서 이동이 가능한 파일보기
  - ln(Link) : 지정한 파일에 대한 심볼링링크나 하드링크를 생성
```shell
cp -rfp 원본파일패스/이름 복사할파일패스/이름 r하위디렉토리포함 f덮어스기 p 실행권한 그대로 복사
rename 변경전파일명 변경후파일명 대상파일
ex)
  touch test1 test2 test3 test4 test5 
  rename test test0 test?


[root@67c211f24ca1 tmp]# ll
total 12
drwxr-xr-x 2 root root 4096 Mar 13 02:17 .
drwxr-xr-x 3 root root 4096 Mar 13 02:15 ..
-rw-r--r-- 1 root root    0 Mar 13 02:11 axt1
-rw-r--r-- 1 root root    0 Mar 13 02:11 axt2
-rw-r--r-- 1 root root    0 Mar 13 02:11 axt3
-rw-r--r-- 1 root root    4 Feb 27 07:33 tmp.txt
[root@67c211f24ca1 tmp]# rename a b axt?
[root@67c211f24ca1 tmp]# ll
total 12
drwxr-xr-x 2 root root 4096 Mar 13 02:17 .
drwxr-xr-x 3 root root 4096 Mar 13 02:15 ..
-rw-r--r-- 1 root root    0 Mar 13 02:11 bxt1
-rw-r--r-- 1 root root    0 Mar 13 02:11 bxt2
-rw-r--r-- 1 root root    0 Mar 13 02:11 bxt3
-rw-r--r-- 1 root root    4 Feb 27 07:33 tmp.txt


```
