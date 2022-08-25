# MetaMask Provider API

- ethereum.isConnected()
  - 현재 연결 되어있는지 true/false의 boolean값으로 반환
- ethereum.enable()
  - 계정 활성화
- ethereum.selectedAddress
  - 선택된 계정 확인



## The default block parameter

- https://ethereum.org/en/developers/docs/apis/json-rpc/
- parameter
  - `HEX String` - an integer block number
  - `String "earliest"` for the earliest/genesis block
  - `String "latest"` - for the latest mined block
  - `String "pending"` - for the pending state/transactions

## EXAMPLES

### eth_getBalance

```javascript
const params = [ window.ethereum.selectedAddress, 'latest']
ethereum.request({method: 'eth_getBalance', params: params}).then(res=>console.log((res,16)*(10**-18)))
```

- 선택된 지갑(계정)의 잔액 조회에 사용
- (res,16) => 결과가 16진법, 10^-18 => 1이더 = 10^18 Wei  