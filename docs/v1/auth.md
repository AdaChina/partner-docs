# 单点登陆(SSO)

## 获取Token

获取学校管理员身份验证Token。Token有效期暂定为24小时。

```
GET /auth/token
```

#### 请求参数

| 名称 | 类型 | 说明 | 必填 | 例子 |
| -- | -- | -- | -- | -- |
| school_id | string | 学校ID | 是 | 1005 |

#### 返回值说明

| 名称 | 类型 | 说明 | 例子 |
| -- | -- | -- | -- |
| token | string | 学校管理员身份Token | ... |
| expires_at | string | Token失效时间 | ... |

#### 请求例子

```
GET /auth/token?school_id=1005
```

#### 响应例子

```json
{
    "token": "eCJ9.eyX0.WkiUzKELZ49eM7oWxAQK_ZXw",
    "expires_at": "2017-02-24T23:52:00+08:00",
}
```

## 跳转学校管理后台

网页端跳转地址。非API请求。

```
GET /auth/sign_in
```

#### 请求参数

| 名称 | 类型 | 说明 | 必填 | 例子 |
| -- | -- | -- | -- | -- |
| token | string | 学校管理员身份Token | 是 | 1005 |

#### 请求例子

```
GET /auth/sign_in?token=eCJ9.eyX0.WkiUzKELZ49eM7oWxAQK_ZXw
```