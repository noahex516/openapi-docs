# Submit order

`POST` /v1/spot/order

## Request Parameters

| name            | location   | type     | required    | Description                                 |
|---------------|------|--------|-------|------------------------------------|
| symbol        | body | string | true  | symbol                                |
| clientOrderId | body | string | false | 客户端ID(最长32位)                       |
| side          | body | string | true  | 买卖方向,[枚举](../README?id=买卖方向)       |
| type          | body | string | true  | 订单type,[枚举](../README?id=订单type)       |
| timeInForce   | body | string | true  | 有效方式,[枚举](../README.md?id=BizType) |
| bizType       | body | string | true  | 业务type,[枚举](../README.md?id=BizType) |
| price         | body | number | false | 价格。现价必填; 市价不填                      |
| quantity      | body | number | false | 数量。现价必填；市价按数量下单时必填                 |
| quoteQty      | body | number | false | 金额。现价不填；市价按金额下单时必填                 |

> Request Example

```shell
curl --location --request POST 'https://api.noahex-test.com/v1/spot/order' \
--header 'Content-Type: application/json' \
--header 'validate-algorithms: HmacSHA256' \
--header 'validate-appkey: 2fa91add-388c-44f2-8365-f4b72886c135' \
--header 'validate-recvwindow: 6000' \
--header 'validate-timestamp: 1725455266041' \
--header 'validate-signature: ce246607785e168d4677afff5af3746eb8513133d11ca3c5e3913eeea5aca63c' \
--header 'Accept: */*' \
--header 'Host: api.noahex-test.com' \
--header 'Connection: keep-alive' \
--data-raw '{"symbol":"BTC_USDT","clientOrderId":"16559590087220001","side":"BUY","type":"LIMIT","timeInForce":"FOK","bizType":"SPOT","price":40000,"quantity":2,"media":"btok","mediaChannel":"12345"}'
```

## Response Result

```json
{
  "code": 0,
  "msg": "success",
  "msgInfo": [],
  "data": {
    "orderId": "401618309946313024",
    "clientOrderId": "16559590087220001"
  },
  "ts": 1725455266831
}
```
