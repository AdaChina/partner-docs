# 学校信息

## 获取学校列表

这里将会返回合作伙伴账号内已授权的学校列表及相关学校信息

```
GET /schools
```

#### 返回值说明

| 名称 | 类型 | 说明 | 例子 |
| -- | -- | -- | -- |
| id | string | 学校ID | 1002 |
| name | string | 学校名称 | 上海市第一小学 |

#### 响应例子

```json
[
    {
        "id": "1002",
        "name": "上海市第一小学"
    },
    {
        "id": "1005",
        "name": "长沙市胜利中学"
    }
]
```