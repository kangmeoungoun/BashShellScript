### 간단 쉘 스크립트
### 간단 쉘 스크립트(4) function
- 함수
  - function 함수명 {
      명령어    
    }
  - 배열 
    - 배열에 숫자 또는 문자 사용 가능
  - 리다이렉션
    - 입력/출력/에러(표준 스트림) 을 지정한 곳으로 바꿔준다.
    - 쉘 스크립트 안에서 텍스트 파일의 활용

```java
#!/bin/bash

function line {
        echo "==================================="
}
line
echo "df result"
df -h
line
echo "free result"
free -m
line
1.라이브러리처럼 사용할 쉘 스크립트 함수


function plus {
echo "$1 + $2 = "
echo $[ $1 + $2 ]
echo
}

function div {
  echo "$1 / $2 = "
  if [ $2 -eq 0 ]
  then
    echo "error 0"
  else
     echo $[ $1 / $2 ]
  fi
  echo
}
source ./calc
plus 30 40
div 30 0
div 10 2


```  