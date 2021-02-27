### 초간단 쉘 스크립트
### 한줄스크립트

- Q1)다음 내용을 한줄로 실행
    - 현재위치에서 tmp디렉토리를 생성
    - tmp디렉토리 안에 tmp.txt 파일을 생성
    - tmp.txt 파이에 tmp라는 내용일 입력
    - tmp.txt 파이르이 내용을 화면에 출력
    
```shell
 mkdir tmp;cd ./tmp; touch tmp.txt; echo tmp >tmp.txt; cat tmp.txt
```
- Q2)cent3 서버의 프로레스 리스트에서 nfs 프로세스를 확인
```shell
ssh cent3 "ps -ef | grep nfs"
```
- Q3) Q2에서 nfs 프로세스의 개수를 확인(grep 제외)
```shell
 ps -efn | grep -c "nfs"
 wc -l
```

- Q4) /var/log 디렉토리 하위에서 message 로그가 있는지 확인하고 있으면 message 로그의 하위 15 라인을 출력
test 문의 조건
  -e : 파일이 존재하는가
  -f : 지정한 파일이 파일이면 참 그외엔 거짓
  -d : 지정한 파일이 디렉토리면 참 그외엔 거짓
```shell
[ -e /var/log/messages ] && tail -n 15 /var/log/messages

```  
- Q5) mount의 결과를 보기 편하게 정렬
  mount | column -t
- Q6) ss의 결과를 보기 편하게 정렬
    ss | cat

결과를 얻는데 필요한 명령어들의 집합 을 파일로 만듦.

