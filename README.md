### 리눅스 명령어
### 실무에서 자주 사용하는 명령어_파일관련_명령어
- 파일 시스템 관련 명령어

  - less : 상하로 커서 이동이 가능한 파일보기 (cat 보다 유용할듯.)
  - ln(Link) : 지정한 파일에 대한 심볼링링크나 하드링크를 생성
    - 하드링크 : 원본파일 을 물리적으로 2개 의 파일을 각각 다른이름으로 하나의 원본파일을 바라보고 있따.(하나를 삭제해도 하나가남아서 원본파일을 읽을수 있다.)
    - 심볼릭 링크 : 윈도우 비유하면 바로가기 원본파일을 가리킨다.(원본을 삭제하면 링크파일은 읽을수 없다.)
```shell
ln -s hardlink.txt  symbolicklink.txt //심볼릭 링크
lrwxrwxrwx 1 root root   12 Feb 21 00:02 symboliclink.txt -> hardlink.txt
l 링크뜻 
hardlink.txt 파일의 이름을 변경하면 symbolicklink.txt 파일은 읽을수가 없다.
```
