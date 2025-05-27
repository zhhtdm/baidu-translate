# baidu translate
封装百度翻译 API，翻译字符串或字符串列表

## 示例
- 同步
```python
from lzhbaidutranslate import baidu_translate

query = 'Hello World! This is 1st sentence. This is 2nd sentence.'
querys = ['Hello World! This is 1st sentence.','This is 2nd sentence.']

# Set your own appid/appkey.
appid = ""
appkey = ""

print(baidu_translate(appid, appkey, query)) # 翻译字符串
print(baidu_translate(appid, appkey, querys)) # 翻译字符串列表
```
- 异步
```python
import asyncio
from lzhbaidutranslate import baidu_translate_async

query = 'Hello World! This is 1st sentence. This is 2nd sentence.'
querys = ['Hello World! This is 1st sentence.','This is 2nd sentence.']

# Set your own appid/appkey.
appid = ""
appkey = ""

async def main():
    print(await baidu_translate_async(appid, appkey, query))
    print(await baidu_translate_async(appid, appkey, querys))

asyncio.run(main())
```

## 安装 - [PyPI](https://pypi.org/project/lzhbaidutranslate/)
```bash
pip install lzhbaidutranslate
```

## API
[Document](https://zhhtdm.github.io/baidu-translate/)


