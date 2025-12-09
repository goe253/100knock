# Day1 - Lambda + API Gateway で Hello API
日付: 2025-12-09

---

## 🎯 今日の目的
- 
- 
- 

---

## 🏗️ 構成図
![Day1 Architecture](img/143638.png)

---

## 📝 手順

### 1. Lambda 関数の作成
1. AWS コンソール → Lambda → 「関数の作成」
2. ランタイム：Python 3.12
3. 関数名：`day1-hello`

---

### 2. Lambda コード編集

```python
import json

def lambda_handler(event, context):
    return {
        "statusCode": 200,
        "body": json.dumps({"message": "Hello from Day1!"})
    }
