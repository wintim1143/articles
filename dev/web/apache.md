# Apache的用法

## ab

ab是一个HTTP服务器的压测工具。

```bash
$ ab -n10000 -c100 http://127.0.0.1:3000/
```

参数。

- `-n`：执行一次测试会话的时候所发出的请求数目，默认是执行一个单一的请求，当然了这样的测试结果也就没什么意义了。
- `-c`：表示“concurrency”，即同时向服务器端发送的请求数目，默认状态下是一次，只执行一个http请求。