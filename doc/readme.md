#### 简介
轻量级文件HTTP服务器

#### 安装[for linux]
```shell

```
#### 配置文件
```yaml
# cat file.yaml
ROOT: /tmp/test
ERROR_LOG: error.log
ACCESS_LOG: access.log
LISTEN: 0.0.0.0:9191
AUTH_USER:
  user1:
    PASSWORD: password1
  user2:
    PASSWORD: password1
```


#### 默认配置
| Key               | Value              |Describe              |
|  ----------       | :-----------:      |   :-----------:      |                    
| ROOT_DIR          | $HOME              |   用户家目录           |
| ERROR_LOG         | error.log          |   日志                |
| ERROR_LOG         | access.log         |   访问日志                |
| LISTEN            | 0.0.0.0:9191       |   监听地址             |


### 请求头参数
| Header               | Value                           |Describe              |
|  ----------       | :-----------:                     |   :-----------:      |                    
| Content-Type      | application/json <br> application/text <br> application/html               |   请求返回类型          |


#### 使用/例如
##### 例子1:
```shell
curl -H "Content-Type:application/json" http://127.0.0.1:9090/
```

##### 例子2:
```shell
curl -H "Content-Type:application/text" http://127.0.0.1:9090/
```

##### 例子3:
```shell
curl -H "Content-Type:application/text" http://127.0.0.1:9090/
```