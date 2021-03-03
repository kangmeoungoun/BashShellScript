### 간단 쉘 스크립트
### 대화식 쉘 스크립트
- 쉘 스크립트 실행 후 사용자에게 입력을 받은 숫자/문자를 처리
- 정해진 숫자 맞추기 게임
```shell

read -[pls] "화면에표시할문자" 변수이름 ::wq      s:secret
read -sp "text input. : " ANY
read -p "text input "  IN

#!/bin/bash
GOAL=$((RANDOM% 100+1))
CNT=0
while [ 1 -eq 1 ]
do
        read -p "text input "  IN
                CNT=$((${CNT} + 1))
        if [ "${IN}" -gt "${GOAL}" ]; then
                echo "UP"
        elif [ "${IN}" -lt "${GOAL}" ]; then
                echo "DOWN"
        else
                echo ${CNT}
                break
        fi
done


exit 0  종료코드 0 :성공 , 1:오류
```