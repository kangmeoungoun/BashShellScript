### 간단 쉘 스크립트
### 

- 정규표현식
    - 텍스트의 패턴을 특수문자 등을 사용하여 표현한것
    
|메타문자|의미|매칭가능한문자열|
|-------|---|--------------|
|A*|A다음에 0개 이상의 문자를 매칭|A Aa Abc A13cg ...|
|A?|A다음에 1개 의 문자를 매칭|A Aa Ab Ac  A1 Az...|
|^A|A로 시작하는 문자열|Abced Avoid Attack ....|
|A$|A로 끝나는 문자열|A bA cdfdA abcdefA|
|A\B|A또는 B가 있음을 의미| cAf cBf|
|[a-z]|a부터z 까지 알파벳의 범위를 매칭| a b c d e ...|



```shell
 ls -1 | grep ^t
find . -type f -name "t*"
sed -n '/$c/p' txt1

```