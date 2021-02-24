### 리눅스 명령어
### 실무에서 자주 사용하는 명령어_검색 /탐색 관련 명령어
- 검색 /탐색 관련 명령어
  - find : 지정한 파일명 또는 정규표현식을 이용하여 파일을 검색
  - which : 환경변수 PATH에 등록된 디렉토리에 잇는 명령어를 찾아주는 도구
  - grep(Global /Regular Expression / print) : 텍스트 검색 기능을 가진 도구 파일이나 표준 입력을 검색하여 지정한 정규 표현식과 맞는 줄을 출력

```shell
find 옵션 찾기시작할패스 익스프레션(name,type,perm) 
find 패스 -name 파일명

which df 
which find

grep 옵션 "찾을문자열" 파일명
grep -ir "error" /var/log/* (i:대소문자구분하지 않는다. ,r:하위디렉토리까지 검색,c:각파일변 찾은문자건수 출력)
```