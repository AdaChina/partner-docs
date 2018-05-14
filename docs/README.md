# 艾道合作伙伴 API 文档

## 当前可用版本
```
V1
```

## API Endpoint
测试环境:
```
待定
```
生产环境:
```
待定
```

## 请求规范
### Header
#### 身份验证

访问 API 时，需提供 API Key 以及 API Secret 进行授权。

Key 和 Secret 格式:
```
key: "dd970b75-75e4-45cf-91d7-a6fc8d399489"
secret: "dJgnOnuZwOrla8IU2GiirUgbNX7HivAjjByHo8E7"
```

#### API版本号

客户端请求时，需指定请求的API版本号

如请求V1版本:

```
Accept: application/vnd.ada-partner.v1+json
```

## 错误信息

如请求出现错误时，将会返回标准HTTP状态码以及应用错误码

[详细应用错误码 (待定)](#)

```
401 Unauthorized
```

```json
{
    "error_code": 1003,
    "message": "未提供认证Header"
}
```
