# 获取单个资产

`GET` /v1/spot/balance

## 请求参数

| 名称       | 位置    | 类型     | 必选 | 说明 |
|----------|-------|--------|----|----|
| currency | query | string | 否  | 币种 |

> 请求示例

```shell
curl --location --request GET 'https://api.noahex-test.com/v1/spot/balance?currency=USDT' \
--header 'validate-algorithms: HmacSHA256' \
--header 'validate-appkey: 2fa91add-388c-44f2-8365-f4b72886c135' \
--header 'validate-recvwindow: 6000' \
--header 'validate-timestamp: 1725534383748' \
--header 'validate-signature: e91e5d4d27d179606b618ae7c728390d32674c660008719cc8a6d09d772d694f' \
--header 'Accept: */*' \
--header 'Host: api.noahex-test.com' \
--header 'Connection: keep-alive'
```

## 响应结果

```json
{
  "code": 0,
  "msg": "success",
  "msgInfo": [],
  "data": {
    "currency": "usdt",
    "currencyId": 11,
    "frozenAmount": "180534.40000000",
    "availableAmount": "8704106.23547842",
    "totalAmount": "8884640.63547842",
    "convertBtcAmount": "156.32640153",
    "convertUsdtAmount": "8884640.6354",
    "withdraw": null
  },
  "ts": 1725534383825
}
```
