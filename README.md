### 간단 쉘 스크립트
### 간단 쉘 스크립트(5) array, redirect
- 함수
  - function 함수명 {
      명령어    
    }
  - 배열 
    - 배열에 숫자 또는 문자 사용 가능
  - 리다이렉션
    - 입력/출력/에러(표준 스트림) 을 지정한 곳으로 바꿔준다.
    - 쉘 스크립트 안에서 텍스트 파일의 활용

  
```shell
test_array=(one two three 4 5 6 7)
for i in $(seq 0 7);do echo ${test_array[${i}]};done
쉘 스크립트에서 배열은 잘 사용하지 않는다.

ls -al txt1 txt2 txt3 1> ok 2> ng

touch report:wq
#rerport 파일 초기화
cp -f /dev/null report
>(overwrite) , >>(append)


touch report
cp -f /dev/null report

{
df -h
pstree
free -m
uptime
} >> report
# result send email

```