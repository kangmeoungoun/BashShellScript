### 간단 쉘 스크립트
### 간단 쉘 스크립트(3) 조건문 반복문
- 반복문
  - for 변수 in 변수에 넣을 데이터
    - do : 데이터가 끝날 때까지 반복해서 실행할 명령어
    - done
  - while 조건문
    - do 조건이 참인 동안 반복해서 실행할 명령어
    - done
  
```shell

#!/bin/bash

#!/bin/bash

for SVR in cent1 cent2 cent3
do
        echo "${SVR}";
done

for NUM in $(seq 1 3)
do
        echo "${NUM}"
done

for NUM in $(cat serverlist)
do
        echo "${NUM}"
done

#!/bin/bash

NUM=1
while [ "${NUM}" -le 3 ]
do
        echo "cent${NUM}"
        NUM=$(( ${NUM} + 1 ))
done

while read SVR
do
        echo ${SVR}
done < serverlist

$(seq 1 3 ) : 명령어 의 결과값 받을때 사용 $()
```
