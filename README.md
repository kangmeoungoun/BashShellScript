### 리눅스 명령어
### 실무에서 자주 사용하는 명령어_기타 관련 명령어
- 기타 명령어
  date : 현재의 날짜와 시간을 출력
  seq : (SEQuence) : 지정한 규칙으로 숫자열을 출력하는 도구
  more : 한 화면씩 지정한 파일의 내용을 출력하는 도구
  watch : 지정한 명령어를 지정한 시간(초)마다 재실행하여 화면에 출력하는 도구
  crontab : 리눅스의 잡 스케줄러의 내용을 출력하거나 편집할 수 있는 도구 명령어라기보단 툴
```shell
date -d '-1day'
week/month/hour/minute/second
date '+%Y-%m-%d-%H:%M:%S'
[root@67c211f24ca1 /]# seq 1 5
1
2
3
4
5
seq -f%02g 1 10
seq -w 1 10

:wwatch date

```