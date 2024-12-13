# Create Orders

`POST` /v1/future-u/trade/v2/order/create

## Request Parameters

| name                 | location   | type     | required    | Description                                                                |
|--------------------|------|--------|-------|-------------------------------------------------------------------|
| clientOrderId      | body | string | false | 自定义orderId                                                        |
| symbol             | body | string | true  | symbol                                                               |
| orderSide          | body | string | true  | 买卖方向：BUY;SELL                                                     |
| orderType          | body | string | true  | 订单type：LIMIT；MARKET                                                 |
| origQty            | body | number | true  | 数量（张）                                                             |
| price              | body | number | false | 价格                                                                |
| positionSide       | body | string | true  | 仓位方向：LONG;SHORT                                                   |
| timeInForce        | body | string | false | 有效方式：GTC;IOC;FOK;GTX                                              |
| triggerPriceType   | body | string | false | 触发价格type：INDEX_PRICE(指数价格); MARK_PRICE(标记价格)；LATEST_PRICE(最新价格， 默认) |
| triggerProfitPrice | body | number | false | 止盈价                                                               |
| triggerStopPrice   | body | number | false | 止损价                                                               |

> Request Example

```shell
curl --location --request POST 'https://api.noahex-test.com/v1/future-u/trade/v2/order/create' \
--header 'Content-Type: application/json' \
--header 'validate-algorithms: HmacSHA256' \
--header 'validate-appkey: 2fa91add-388c-44f2-8365-f4b72886c135' \
--header 'validate-recvwindow: 60000' \
--header 'validate-timestamp: 1725606650399' \
--header 'validate-signature: e25fd957e26976c481c55ef55dee0c1db42eb26d8d855d8e2f0720a01d27e81d' \
--header 'Accept: */*' \
--header 'Host: api.noahex-test.com' \
--header 'Connection: keep-alive' \
--data-raw '{"clientOrderId":"1232323232","symbol":"btc_usdt","orderSide":"BUY","orderType":"MARKET","origQty":10,"positionSide":"LONG","timeInForce":"IOC","triggerPriceType":"INDEX_PRICE"}'
```

## Response Result

```json
{
  "code": 0,
  "msg": "success",
  "msgInfo": null,
  "data": "402253259192112000",
  "ts": 1725606650522
}
```
