### 간단 쉘 스크립트
### 
- awk 
    - sed 기능 + 변수/함수/연산자를 사용하여 필요한 데이터를 제어할 수 있는 커맨드
        - awk 옵션 읽어들일_파일명
    
|옵션|설명|
|----|---|
|-F 필드구분자|필드를 구분하기 위한 구분자를 지정|
|-f 파일이름| awk프로그램이 읽어들일 파일 이름을 지정|
|-변수=변수값|awk프로그램에서 사용할 변수를 지정|
```shell

 awk '{print $1}' txt13
awk '/ccc/{print $1}' txt13 #ccc 라는 문자열을 찾고 싶을때



aaa     111     zzz
bbb     222     xxx
ccc     333     yyy
ddd     444     qqq
eee     555     ddd

# 111 이 있는줄에 세번째필드 zzz 출력하기
grep '111' txt13 | awk '{print $3}'
awk '/111/{print $3}' txt13

aaa:111:zzz
bbb:222:xxx
ccc:333:yyy
ddd:444:qqq
eee:555:ddd
cat colon_txt13 | awk '{split($0,arr,":"); print arr[3]}'
awk -F: '{print $1}' colon_txt13

uptime | awk '{print $10 $11 $12}' | awk -F, '{print $1, $2, $3}'

df -h | awk -F%  '{print $2}' | sed -n '5p' # 특정 라인 출력 p
```