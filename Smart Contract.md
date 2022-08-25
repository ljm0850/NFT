# Smart Contract

- 디지털 형식으로 명시된 서약(commitment)들의 집합
- 단순 컴퓨터 프로그램



### 블록체인에서의 Smart Contract

- 불변의 컴퓨터 프로그램
  - 배포되면 변경 불가
  - 실행한 결과가 모두 같음
  - EVM(ethereum virtual machine) 위에서 동작
  - 모든 컴퓨터에서 동일한 상태 유지
- Smart Contract 작성 언어
  - Solidity
  - LLL
  - Viper
  - Assembly



### 배포 & 호출 순서

1. Smart Contract Code를 컴파일
2. EVM Bytecode, ABI in JSON 트랜잭션 생성
   - Bytecode : Solidity등으로 작성된 스마트 컨트랙트 코드
   - Application Binary Interface(ABI) :  응용 프로그램과 운영 체제 또는 응용 프로그램과 해당 라이브러리, 마지막으로 응용 프로그램의 구성요소 간에서 사용되는 낮은 수준의 인터페이스
3. 서명



## Remix

- 스마트 컨트랙트 IDE

  