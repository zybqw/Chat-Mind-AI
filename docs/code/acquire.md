# requests

这是一个示例基础代码，所有示例代码均会使用如下函数：

> 代码未经测试，请谨慎使用

```python
from functools import wraps
from time import sleep
from typing import Any, Callable, Dict, List, Optional

import requests
from requests.exceptions import ConnectionError, HTTPError, RequestException, Timeout

HEADERS = {
    "Content-Type": "application/json",
    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36 Edg/124.0.0.0",
}
BASE_URL = "https://x.chatmindai.net/api"

def retry(retries: int = 3, delay: float = 1) -> Callable:
    if retries < 1 or delay <= 0:
        raise ValueError("Are you high, mate?")

    def decorator(func: Callable) -> Callable:
        @wraps(func)
        def wrapper(*args, **kwargs) -> Any:
            for i in range(1, retries + 1):

                try:
                    return func(*args, **kwargs)
                except Exception as e:

                    if i == retries:
                        print(f"Error: {repr(e)}.")
                        print(f'"{func.__name__}()" failed after {retries} retries.')
                        break
                    else:
                        print(f"Error: {repr(e)} -> Retrying...")
                        sleep(delay)

        return wrapper

    return decorator

def update_token(token):
    global HEADERS
    HEADERS["Authorization"] = f"Bearer {token}"

def send_request(
        url: str,
        method: str,
        params: Optional[Dict] = None,
        data: Any = None,
        headers: Dict = None,
        sleep: int = 0.3,
    ) -> Optional[Any]:

        headers = headers or HEADERS
        url = url if "http" in url else f"{BASE_URL}{url}"
        time.sleep(sleep)
        try:
            response = session.request(
                method=method, url=url, headers=headers, params=params, data=data
            )
            response.raise_for_status()
            return response
        except (HTTPError, ConnectionError, Timeout, RequestException) as err:
            print(f"错误码: {response.status_code} 错误信息: {response.text}")
            print(f"网络请求异常: {err}")
            return response

```
