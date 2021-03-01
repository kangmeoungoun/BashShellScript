### 간단 쉘 스크립트
### 간단 쉘 스크립트(1) 조건문 case
- 조건문
  - Case 변수 in
    - 패턴 1) : 패턴 1이 참일 경우 실행할 명령어;;
    - 패턴 2) : 패턴 2가 참일 경우 실행할 명령어;;
    - *) : 위에서 지정한 모든 패턴이 해당이 안되는 경우 실행할 명령어;; 
  - esac  
```shell

./nginx_ctl.sh a b c 
### $1 : a ,$2 : b, $3 : c


## ./nginx_ctl.sh start      : nginx start
## ./nginx_ctl.sh stop       : ntinx stop
## ./nginx_ctl.sh reload     : nginx reload
## ./nginx_ctl.sh configtest : nginx.conf check
CMD=$1

case "${CMD}" in
start)
        echo start;;
stop)
        echo stop;;
reload)
        echo reload;;
configtest)
        echo configtest;;
*)
        echo "./nginx_ctl.sh {staart|stop|reload|configtest}";;
esac

```