# 概要

Spring Boot のチュートリアルとして簡単な REST API を作りました。

作ったものを以下に記述します。

## hello world を返す API

パス: /hello
HTTPメソッド: GET
ステータスコード: 成功時 200
レスポンスの例:
```json
{
    "greeting": "Hello , World",
    "timestamp": "2024-05-13T07:21:10.882186+09:00"
}
```

## dog の List を返すAPI

パス: /dogs
HTTPメソッド: GET
ステータスコード: 成功時 200
レスポンスの例:
```json
[
    {
        "name": "Pochi",
        "age": 5
    },
    {
        "name": "Taro",
        "age": 10
    }
]
```
# 動作確認

API の仕様通りのレスポンスが得られました。

```
Response Headers
Content-Type: application/json
Transfer-Encoding: chunked
Date: Sun, 12 May 2024 22:31:03 GMT
Keep-Alive: timeout=60
Connection: keep-alive

Response Body
{"greeting":"Hello , World","timestamp":"2024-05-13T07:31:03.99879+09:00"}
```
```
Response Headers
Content-Type: application/json
Transfer-Encoding: chunked
Date: Sun, 12 May 2024 22:25:49 GMT
Keep-Alive: timeout=60
Connection: keep-alive

Response Body
[{"name":"Pochi","age":5},{"name":"Taro","age":10}]
```

