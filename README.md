# wechat_python_sdk
Tencent wechat python sdk, originate from author: piglei2007@gmail.com

# How to use
```
code = request.GET.get('code')
client = WXAPIClient(WX_AKEY, WX_SKEY, redirect_uri=WX_CALLBACK_URL)
access_token = client.request_access_token(code)
client.set_access_token(access_token['access_token'], access_token['expires_in'])
openid = access_token['openid']

```
