### 리눅스 명령어
### 실무에서 자주 사용하는 명령어_파일관련_명령어
- 파일 관련 명령어
  - paste : 지정한 파일들의 행을 읽어 탭으로 구분하여 병합
  - dd(Dataset Definition) : 블록 단위로 데이터셋을 정의하여 파일을 쓰고 읽음
    - 랜덤데이터로 파일을 생성하거나 그 파일을 생성한 시간을 측정해서 드라이버의 성능체크
  - tar (Tape Archive) : 지정한 데이터 및 디렉토리를 하나의 파일로 만듦 (압축)
```shell
paste txt1 txt2
aaa     111
bbb     222
ccc     333
ddd     444
eee     555

vi ~/.bashrc
alias 등록
source ~/.bashrc 적용

dd if=인풋파일이름 of=아웃풋파일이름 bs=바이트(크기) count=블럭을복사할횟수
dd if=/dev/urandom of=ddtest2 bs=1024 count=1024
ddtest2 라는 이름의로 1.0M 랜덤문자 파일 생성

tar -cvzf 생성할파일명 압축할디렉토리명/파일명   압축할떄 (c=create,v=verbos(말많은) 실행과정을 전부 화면출력,z=gzip 으로 압축한다. f=파일이름을 명시적으로 지정해주는옵션)
tar -xvzf 파일명    압축풀떄 (x =extract(추출하다))
tar -tf 파일명 (압출파일리스트 볼때) 

tar -cvzf work.tgz ./work work.tgz 파일로 압축하겠다  ./work 폴더를   .tgz tar 로 gzip 압축했다 암묵적으로 사용

tar -tf work.tgz
./work/
./work/ddtest2
./work/ddtest
./work/txt1
./work/txt2
   
tar -xvzf work.tgz 
```