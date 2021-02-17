### 리눅스와 쉘
#### 리눅스의 종류
- 리눅스 배포판
    - 데비안 계열 : 우분투,민트 ,칼리 등(초보자 접하기 비교적 쉽고 인터페이스 예쁘다. 칼리리눅스는 해킹용 툴이 만이 들어가있다.)
    - 슬랙웨어 계열 : 오픈수세
    - 젠투  (가장 마이너한 리눅스,극소수 사람들이 사용)
    - 레드햇 계열 : 페도라, CentOs(리눅스 최조로 유료서비스 시작한 레드햇 계열,배포무료 서비스지원 유료,
      AWS 또 레드햇 계열, 페도라 :업데이트 레드햇 계열 리눅스중 가장 빠르다. CentOs:레드햇 안정적인 버전 유료 패키지 버전 제거,무료
      ,서비스지원x
    )         
- 맥 OS 또는 Unix BSD계열
#### 쉘의 종류
|쉘 이름|특징|실행시 참조 파일|프로그램 
|----------------|--------------|----------|-------|
|sh(Bourne Shell)|최조의 유닉스 쉘|~/.profile|/bin/sh| 
|csh(C Shell)|Unix BSD 를 위해 배포|~/.cshrc|/bin/sh| 
|ksh(Korn Shell)|csh 보다 빠르고 sh로 작성된 스크립트와 호환|~/.ksh|/bin/sh| 
|**bash(Bourne-Again Shell)**|GNU 프로젝트의 리눅스 기본 쉘 본쉘을 대체/호한|~/.etc/profile /etc/bashrc ~/.bash_profile ~/.profile ~/.bashrc|/bin/sh|

#### GUI와 CLI
- GUI Graphic User Interface X-Window(X11)을 사용
- CLI Command-Line Interface 텍스트로만 화면을 표시
- CLI 를 사용하는 이유:그래픽이 차지하는 리소스르 줄이기 위해. 
```shell


```
