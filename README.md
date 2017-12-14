# URL2io Python SDK

This is the URL2io python SDK suite. Note that python3 is required.

[API Docs](http://www.url2io.com/docs)

## 1. url2io.py

This is the underlying API implementation.

How to use? example:

1. [register](http://www.url2io.com/accounts/register) and get **`token`**
2. coding

```python
>>> import url2io
>>> api = url2io.API(token)
>>> # get content and next page link
>>> ret = api.article(url='http://www.url2io.com/products', fields=['next',])
>>> print(ret)
{
    u'content': u'<div><p>\u63d0\u4f9b\u7b80\u5355\uff0c',
    u'date': None,
    u'title': u'URL2io \u4ecb\u7ecd',
    u'url': u'http://www.url2io.com/products'
}
```

[more detial](http://blog.url2io.com/url2io-python-sdk/example%20show%20how%20to%20use%20SDK/)
