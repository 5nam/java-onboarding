# 미션 - 온보딩

## 🔍 진행 방식

- 미션은 **기능 요구 사항, 프로그래밍 요구 사항, 과제 진행 요구 사항** 세 가지로 구성되어 있다.
- 세 개의 요구 사항을 만족하기 위해 노력한다. 특히 기능을 구현하기 전에 기능 목록을 만들고, 기능 단위로 커밋 하는 방식으로 진행한다.
- 기능 요구 사항에 기재되지 않은 내용은 스스로 판단하여 구현한다.

## 📮 미션 제출 방법

- 미션 구현을 완료한 후 GitHub을 통해 제출해야 한다.
    - GitHub을 활용한 제출 방법은 [프리코스 과제 제출](https://github.com/woowacourse/woowacourse-docs/tree/master/precourse) 문서를 참고해
      제출한다.
- GitHub에 미션을 제출한 후 [우아한테크코스 지원](https://apply.techcourse.co.kr) 사이트에 접속하여 프리코스 과제를 제출한다.
    - 자세한 방법은 [제출 가이드](https://github.com/woowacourse/woowacourse-docs/tree/master/precourse#제출-가이드) 참고
    - **Pull Request만 보내고 지원 플랫폼에서 과제를 제출하지 않으면 최종 제출하지 않은 것으로 처리되니 주의한다.**

## 🚨 과제 제출 전 체크 리스트 - 0점 방지

- 기능 구현을 모두 정상적으로 했더라도 **요구 사항에 명시된 출력값 형식을 지키지 않을 경우 0점으로 처리**한다.
- 기능 구현을 완료한 뒤 아래 가이드에 따라 테스트를 실행했을 때 모든 테스트가 성공하는지 확인한다.
- **테스트가 실패할 경우 0점으로 처리**되므로, 반드시 확인 후 제출한다.

### 테스트 실행 가이드

- 터미널에서 `java -version`을 실행하여 Java 버전이 11인지 확인한다. 또는 Eclipse 또는 IntelliJ IDEA와 같은 IDE에서 Java 11로 실행되는지 확인한다.
- 터미널에서 Mac 또는 Linux 사용자의 경우 `./gradlew clean test` 명령을 실행하고,   
  Windows 사용자의 경우  `gradlew.bat clean test` 명령을 실행할 때 모든 테스트가 아래와 같이 통과하는지 확인한다.

```
BUILD SUCCESSFUL in 0s
```

---

## 🚀 기능 요구 사항
아래의 7가지 기능 요구 사항을 모두 해결해야 한다.

1. [문제 1](./docs/PROBLEM1.md)
2. [문제 2](./docs/PROBLEM2.md)
3. [문제 3](./docs/PROBLEM3.md)
4. [문제 4](./docs/PROBLEM4.md)
5. [문제 5](./docs/PROBLEM5.md)
6. [문제 6](./docs/PROBLEM6.md)
7. [문제 7](./docs/PROBLEM7.md)

---

## 문제별 구현 기능
### 문제 1 기능
- 페이지 각 자리수를 int 배열로 만드는 기능
- 페이지 각 자리수를 더하는 기능
- 페이지 각 자리수를 곱하는 기능
- 더 큰 수를 리턴하는 기능
- 입력된 페이지 수가 홀수, 짝수 순이면서 차이가 ‘1’ 인지 체크하는 기능 : 예외체크
- 숫자를 비교하여 포비 승 → 1 | 크롱 승 → 2 | 무승부 → 0 리턴하는 기능

### 문제 2 기능
- String 을 ArrayList 로 변환하는 기능
- ArrayList 를 String 으로 변환하는 기능
- 연속 중복되는 문자를 찾는 기능
- 중복되는 문자열을 삭제하는 기능

### 문제 3 기능
- number 을 배열에 1 ~ number 까지 나열하는 기능
- 두 자리 이상의 숫자를 int[] 로 분리하는 기능
- 배열에 3, 6, 9 가 들어있는지 탐색한 후 최종 개수를 반환하는 기능
- 각 숫자마다 3, 6, 9 가 몇 번 들어가는지 판단하고, 그 개수를 리턴하는 함수

### 문제 4 기능
- 입력받은 String 을 char[] 로 변환하는 기능
- 대문자인지, 소문자인지 판단하는 기능
- 문자를 규칙에 맞게 변환하는 기능
  1. char 타입의 input 을 매개변수로 받아온다.
  2. input 이 대문자일 경우, input 에서 'A'를 뺀다.
  3. ('Z' - 뺀 결과)를 리턴한다.
  4. input 이 소문자일 경우, input 에서 'a' 를 뺀다.
  5. ('z' - 뺀 결과)를 리턴한다.
  6. input 이 공백일 경우에는 그냥 리턴한다.

### 문제 5 기능
- 리스트를 0 으로 초기화하는 기능
- 규칙에 맞게 돈을 반환하는 기능

### 문제 6 기능
- 닉네임만 모아서 String 배열로 반환하는 기능
- 닉네임을 두 글자씩 쪼개서 String 배열에 저장해서 리턴하는 기능
  ex) 제이엠 : 제이, 이엠
- 닉네임끼리 연속으로 겹치는 부분이 있는지 찾는 기능
  - 닉네임을 두 글자씩 쪼갠 배열(기준) 과 비교 대상 닉네임을 쪼개 배열을 받고, 각각 2 글자씩 비교함
  ex) 제이, 이엠 과 엠제, 제이를 차례로 비교
    1. 제이 == 엠제
    2. 제이 == 제이 -> 일치하므로 true 리턴
- 결과 이메일 리스트의 중복을 제거하는 기능
- 결과 이메일 리스트를 오름차순 정렬하는 기능

### 문제 7 기능 목록
- 친구 목록에서 원하는 대상 찾기 기능 

  : `target` 과 일치하는 친구를 찾기 위한 기능

- 리스트에 중복을 제거하는 기능

  : 

- 점수 부여하는 기능
  
  : `result` (점수를 반영할 리스트)와 `freindName` (점수를 반영할 친구), `score`(더해질 점수) 를 매개변수로 받아와서 점수 업데이트

- 정렬하는 기능
  
  : 점수가 가장 높은 순으로 정렬, 점수가 같으면 이름 순으로 정렬

---

## 🎯 프로그래밍 요구 사항

- JDK 11 버전에서 실행 가능해야 한다. **JDK 11에서 정상적으로 동작하지 않을 경우 0점 처리한다.**
- `build.gradle`을 변경할 수 없고, 외부 라이브러리를 사용하지 않는다.
- 프로그램 종료 시 `System.exit()`를 호출하지 않는다.
- 프로그램 구현이 완료되면 `ApplicationTest`의 모든 테스트가 성공해야 한다. **테스트가 실패할 경우 0점 처리한다.**
- 프로그래밍 요구 사항에서 달리 명시하지 않는 한 파일, 패키지 이름을 수정하거나 이동하지 않는다.

---

## ✏️ 과제 진행 요구 사항

- 미션은 [java-onboarding](https://github.com/woowacourse-precourse/java-onboarding) 저장소를 Fork & Clone해 시작한다.
- 과제 진행 및 제출 방법은 [프리코스 과제 제출](https://github.com/woowacourse/woowacourse-docs/tree/master/precourse) 문서를 참고한다.
