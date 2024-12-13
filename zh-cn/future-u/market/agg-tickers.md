# 获取全交易对的聚合行情信息

`GET` v1/future-u/market/public/q/agg-tickers


## 请求参数

注：此方法不需要签名

> 请求示例
```shell
curl --location --request GET 'https://api.noahex-test.com/v1/future-u/market/public/q/agg-tickers' \
--header 'Accept: */*' \
--header 'Host: api.noahex-test.com' \
--header 'Connection: keep-alive'
```

## 响应结果

```json
{
  "code": 0,
  "msg": "success",
  "msgInfo": null,
  "data": [
    {
      "t": 1721494477587,
      "s": "trb_usdt",
      "c": "97.3054",
      "h": "97.3054",
      "l": "97.3054",
      "a": "10",
      "v": "97",
      "o": "97.3054",
      "r": "0.0000",
      "i": "80.6803",
      "m": "99.1639",
      "bp": "97.3054",
      "ap": "101"
    },
    {
      "t": 1725508903642,
      "s": "eth_usdt",
      "c": "2402.97",
      "h": "2488.36",
      "l": "2369.94",
      "a": "55812970",
      "v": "1359163481",
      "o": "2439.10",
      "r": "-0.0148",
      "i": "2404.26",
      "m": "2403.18",
      "bp": "2402.94",
      "ap": "2402.97"
    },
    {
      "t": 1725508903642,
      "s": "btc_usdt",
      "c": "57082.95",
      "h": "58498.95",
      "l": "56156.15",
      "a": "532399999",
      "v": "3058417182",
      "o": "57702.70",
      "r": "-0.0107",
      "i": "57112.33",
      "m": "57084.64",
      "bp": "57082.9",
      "ap": "57083.0"
    },
    {
      "t": 1725508903642,
      "s": "sol_usdt",
      "c": "131.397",
      "h": "134.846",
      "l": "126.887",
      "a": "32900571",
      "v": "433682175",
      "o": "126.887",
      "r": "0.0355",
      "i": "131.454",
      "m": "131.397",
      "bp": "131.38",
      "ap": "131.383"
    },
    {
      "t": 1721494488597,
      "s": "doge_usdt",
      "c": "0.108000",
      "h": "0.108000",
      "l": "0.108000",
      "a": "331",
      "v": "35",
      "o": "0.108000",
      "r": "0.0000",
      "i": "0.133194",
      "m": "0.132751",
      "bp": "0.1076",
      "ap": "0.108"
    },
    {
      "t": 1721494477588,
      "s": "ordi_usdt",
      "c": "30.00",
      "h": "30.00",
      "l": "30.00",
      "a": "13",
      "v": "390",
      "o": "30.00",
      "r": "0.0000",
      "i": "41.05",
      "m": "40.87",
      "bp": "28.52",
      "ap": "31.53"
    },
    {
      "t": 1723800486231,
      "s": "bnb_usdt",
      "c": "567.74",
      "h": "568.66",
      "l": "567.41",
      "a": "80441",
      "v": "456485",
      "o": "568.66",
      "r": "-0.0016",
      "i": "522.32",
      "m": "567.77",
      "bp": "567.69",
      "ap": "567.71"
    },
    {
      "t": 1723793625584,
      "s": "1000shib_usdt",
      "c": "0.016325",
      "h": "0.016337",
      "l": "0.016316",
      "a": "52771",
      "v": "86157",
      "o": "0.016335",
      "r": "-0.0006",
      "i": "0.013446",
      "m": "0.016324",
      "bp": "0.016322",
      "ap": "0.016323"
    },
    {
      "t": 1723800486241,
      "s": "trx_usdt",
      "c": "0.13562",
      "h": "0.13562",
      "l": "0.13562",
      "a": "500",
      "v": "135",
      "o": "0.13562",
      "r": "0.0000",
      "i": "0.13160",
      "m": "0.12",
      "bp": "0.13562",
      "ap": "0.13563"
    },
    {
      "t": 1723793625584,
      "s": "xrp_usdt",
      "c": "0.6136",
      "h": "0.6140",
      "l": "0.6136",
      "a": "98883",
      "v": "60695",
      "o": "0.6140",
      "r": "-0.0006",
      "i": "0.5676",
      "m": "0.6136",
      "bp": "0.6135",
      "ap": "0.6137"
    }
  ],
  "ts": 1725508905401
}
```
