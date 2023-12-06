# DICE Git Guide

## 목차

[1. Commit Message]()

<hr />

<br />

## 1. Commit Message

### 작업 종류에 따라서 분류 합니다.

작업 종류에 따라 커밋 메시지의 가장 앞 부분을 분류합니다.

- feat : 새로운 기능을 추가했을 경우 사용합니다.
- fix : 올바르지 않은 기능을 수정했을 경우 사용합니다.
- doc : md, sql 등의 코드가 아닌 파일을 추가했을 경우 사용합니다.
- remove : 특정 코드 및 파일을 삭제했을 경우 사용합니다.
- rename : 파일, 폴더의 이름을 수정하거나 경로를 변경하는 경우 사용합니다.
- refactor : 코드를 리팩토링 하는 경우 사용합니다.
- comment : 주석을 추가하거나 수정하는 경우 사용합니다.
- test : 테스트 코드와 관련된 작업을 하는 경우 사용합니다.
- style : lint, format을 실행할 경우 사용합니다.

<br />

### 명령어로 작성합니다.

commit message는 명령어로 작성해야하고, 첫 글자는 대문자로 작성합니다. 예를 들어 Login API를 추가했다고 가정했을 경우 아래와 같이 작성합니다.

```
feat : Add Login API
```

<br />

### 부정의 의미를 나타낼 때는 No가 아닌 Don't을 사용합니다.

Login API에서 로그인 기록을 더이상하지 않는 작업을 할 떄는 아래와 같이 작성하면 됩니다.

```
feat : Don't use recording login log
```

<br >

### 관사는 사용하지 않습니다.

소셜 회원가입 할 때 Google을 더이상 지원하지 않게 수정했다고 하더라도 a, an, the와 같은 관사를 사용하지 않습니다.

```
fix : Don't support Google Login
```

<br />

### 특정 코드를 수정 했을 경우 자세하게 작성합니다.

단순하게 코드를 수정할 때 'fix : Login logic'와 같이 간단하게 작성하는 것이 아닌 로직 중에서 어디를 어떻게 구쳤고 어떤 결과가 되었고 어떤 이슈가 발생하고 있었는 지등을 간략하게라도 담습니다.

- 로그인 로직 중에서 비밀번호 암호화 유효성 검사의 Key를 변경합니다.

  ```
  fix : Change Key of password encryption validation in login logic
  ```

<br />

- 회원가입 기록 추적을 위해 회원가입 로직을 수정합니다.

  ```
  fix : Revise membership logic to track membership records
  ```
