# Cookie
## 浏览器读取与写入
参考：[Cookie.md](../JavaScript/操作浏览器/Cookie.md)

## 服务器端读取与写入
1. 安装相关模块，解析 Cookie

```bash
npm install cookie-parser
```

2. Express 写入 Cookie 到响应中，并设置[相关参数](http://expressjs.com/en/5x/api.html#res.cookie)

```js
var cookieParser = require('cookie-parser');
// ...
app.use(cookieParser());
res.cookie(name, value, [, options]);
```

常用参数 option 设置：
* `maxAge` Cookie 的有效期，以毫秒计算
* `httpOnly` 仅可以通过 http 传输，布尔值

3. Express 读取 Client 端发送的请求中的 Cookie

```js
// ...
req.cookies.yourCookieName;
```
