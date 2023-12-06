# Dice Typescript Guide

## 목차

[1. Namaing](#1-namaing)
[2. 변수](#2-변수)

<hr />

<br />

## 1. Namaing

변수, 함수 등의 Naming 규칙에 대해 기술합니다.

<br />

### 변수와 함수는 Camel Case를 사용합니다.

기본적으로 변수와 함수는 Camel Case를 사용하여 작성합니다.

```typescript
const userAge = 20;
const getUserAge = () => {
  return 20;
};
```

<br />

### 상수는 Snake Case를 사용합니다.

상수란 const로 선언하는 것이 아닌 프로젝트 내부에서 환경 변수와 같이 변하지 않는 값을 의미합니다. 상수를 선언할 때는 const를 사용하여 대문자와 Snake Case로 구성합니다.

```typescript
const SERVER_URL = localhost:8080;
const DATABASE_USERNAME = "admin";
```

<br />

### Class와 interface ENUM은 Pascal Case를 사용합니다.

```typescript
Class Person {}

interface LoginParams {}

enum MemberType {}
```

<br />

## 2. 변수

<br />

### var를 사용하지 않습니다.

변수를 선언할 때는 가능한 const를 사용하고, 재할당이 필요할 경우에만 let을 사용합니다.

<br />

### 변수는 사용하는 시점에 선언 및 할당을 합니다.

변수를 사용하는 시점에서 선언 및 할당을 해주며 맨위에 같이 몰아서 작성하지 않습니다.

```typescript
const name = "김인후";

console.log(name);

const age = 23;

console.log(age);
```

<br />

### const와 let이 같은 위치에 있다면 const를 더 위에 작성합니다.

```typescript
const age = 23;
const name = "김인후";
let year = "2023";
```
