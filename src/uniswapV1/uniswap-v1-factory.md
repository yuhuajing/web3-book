# Uniswap V1
- 仅支持创建 `ETH-Token` 的交易对
- 同个交易池中只能进行 `ETH/Token` 的兑换
- 不同 `Token` 的兑换，需要不同交易池的参与
```solidity
@public
def createExchange(token: address) -> address:
    assert token != ZERO_ADDRESS
    assert self.exchangeTemplate != ZERO_ADDRESS
// 当前Token未创建过交易池
    assert self.token_to_exchange[token] == ZERO_ADDRESS
// 创建交易池
    exchange: address = create_with_code_of(self.exchangeTemplate)
// 记录交易对合约地址
    Exchange(exchange).setup(token)
    self.token_to_exchange[token] = exchange
    self.exchange_to_token[exchange] = token
    token_id: uint256 = self.tokenCount + 1
    self.tokenCount = token_id
    self.id_to_token[token_id] = token
    log.NewExchange(token, exchange)
    return exchange
```