### 간단 쉘 스크립트
### 메뉴 구성
- 메뉴가 있는 쉘 스크립트
    - dialog --옵션명 옵션에 필요한 변수
      
|    옵션  |        설명            |  옵션   |            설명             | 
|---------|---------------------- |---------|----------------------------|
| calendar|날짜를 선택하는 달력을 표시| gouge   |진행 비율을 나타는 진행바를 표시|   
| cheklist|여러 항목의 선택이 가능한 체크박스를 표시| infobox   |메세지를 표시|   
| radiolist|한 가지 항목만 선택이 가능한 라디오버튼을 표시| menu   |선택할 수 있는 목록을 표시|   
| fselect|파일을 선택하는 창을 표시| msgbox|메시지를 표시하고 ok 버튼을 표시|
| passwordbox|입력받는 텍스트를 숨기는 입력 창을 표시| yesno|메시지를 표시하고 yes,no 버튼을 표시|

```shell
#1. uptime
#2. df -h
#3. free -m
#4. pstree
#5. 서버를 입력받아서 그 서버에 ssh 로 접속

# 함수
# clear
# txt 로 메뉴를 출력

#!/bin/bash

function menu {
  clear
  cat << EOF
  ============= MENU ===============
  1. uptime
  2. df
  3. free
  4. pstree
  5. ssh connect
  6. menu exit
  =================================
EOF
  read -p "menu choice : " SELECT
}
function press_key {
  echo
  read -n1 -rsp "press any key to continue..."
  echo
  ehco

}
while true
do
  menu
  case ${SELECT} in
    1)
        clear
        echo " uptime "
        uptime
        press_key
        ;;
    2)
        clear
        echo " df "
        df -h
        press_key
        ;;
    3)
        clear
        echo " free "
        free -m
        press_key
        ;;
    4)
        clear
        echo " pstree "
        pstree
        press_key
        ;;
    6)
        exit 0;;
    *)
        echo "wrong number"
        press_key
        ;;

  esac
done

```


      