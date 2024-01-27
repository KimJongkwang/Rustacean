# cargo

- node의 npm같은 패키지 관리 도구
- 복잡한 프로젝트시 `rustc` 컴파일러보다 디펜던시나 확장에 유용

## cargo command basic

### 프로젝트 생성
```
cargo new project name
```

### 프로젝트 빌드

#### debug build
```
cargo build
```
- target/debug에 컴파일 파일이 저장
- 코드 benchmark시 사용

#### release build
```
cargo build --release
``` 
- 옵션추가시 target/release에 최적화하여 컴파일
- build시 최적화를 통해 코드실행 성능이 좋음
- 하지만 최적화때문에 컴파일 시간이 오래 걸림

### 프로젝트 실행
```
cargo run #running target/debug/proejct_name
```

### 컴파일 체크
```
cargo check
```

- 컴파일 가능여부 체크. 컴파일 해주지는 않음
- build 보다 빠르게 컴파일 가능한 코드인지 판단해주기 때문에, 에러를 찾는데 build 명령어보다 빠름
