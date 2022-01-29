#### LANGUAGE 
[中文](https://github.com/wanggaolin/go-fileHttp#readme)
[English](https://github.com/wanggaolin/go-fileHttp/blob/master/doc/readme_zh.md)
#### 简介
轻量级文件HTTP服务器

![这是图片](doc/demo.png "Magic Gardens")

#### 安装[for linux]
```shell

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
curl -H "Content-Type:application/text" http://127.0.0.1:9090/
curl -H "Content-Type:application/text" http://127.0.0.1:9090/
```
