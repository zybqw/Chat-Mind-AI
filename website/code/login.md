# 登录

以下是一个示例程序：

> 代码未经测试，请谨慎使用

```python
import json

import .acquire as Acquire

acquire = Acquire

def login(phonenum: int, password: str):
    data = json.dumps({"phonenum": phonenum, "password": password})
    response = acquire.send_request(
        url="https://x.chatmindai.net/api/user/login", method="post", data=data
    )
    return response.json()

res = ai.Login().login(password="114514", phonenum=1919810)
tok = res["data"]["token"]
acuqire.update_token(res["data"]["token"])

```
