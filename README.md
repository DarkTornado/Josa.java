# Josa.java

© 2021 Dark Tornado, All rights reserved.

* 마지막 글자 보고 알아서 조사 붙여주는 소스
* 다른 언어로도 구현되면 레포 이름 바뀔 듯?

## 사용법?
* `Josa.java` 파일 받아서 패키지명 적당히 수정하거나, 똑같은 패키지 만들어서 추가
* Josa.getJosa(String str, int type);로 적절한 조사 반환 가능
* 예시
```java
String word = "시험";
System.out.println("이번 " + word + Josa.getJosa(word, Josa.TYPE_은는) + " 어려웠다.");
//출력결과 : 이번 시험은 어려웠다.
```

## type 상수 목록
### int Josa.TYPE_은는
* `~은`과 `~는` 중 적절한 조사 선택. 값은 `0`
### int Josa.TYPE_이가
* `~이`와 `~가` 중 적절한 조사 선택. 값은 `1`
### int Josa.TYPE_을를
* `~을`과 `~를` 중 적절한 조사 선택. 값은 `2`
### int Josa.TYPE_이
* `~(이)라고`와 같이, 사이에 `~이`를 붙일지 말지 선택. 값은 `3`
### int Josa.TYPE_으
* `~(으)로`와 같이, 사이에 `~으`를 붙일지 말지 선택. 값은 `4`
