#### LANGUAGE 
[English](https://github.com/wanggaolin/go-fileHttp#readme)
[中文](https://github.com/wanggaolin/go-fileHttp/blob/master/doc/readme_zh.md)

#### 简介
轻量级文件HTTP服务器

![demo photo](doc/demo.png "Magic Gardens")

#### 安装
##### [for linux]
```shell
git clone https://github.com/wanggaolin/go-fileHttp.git && cd go-fileHttp && ./file_http
```
##### [for mac]
```shell
wget https://github.com/wanggaolin/go-fileHttp/archive/refs/tags/mac-v1.0.tar.gz
tar -xvf mac-v1.1.tar.gz
cd go-fileHttp-mac-v1.1   
./file_http
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
##### 获取文件列表:
```shell
curl -H "Content-Type:application/json" http://127.0.0.1:9090/
curl -H "Content-Type:application/text" http://127.0.0.1:9090/
curl -H "Content-Type:application/html" http://127.0.0.1:9090/
```

##### 下载文件:
```shell
wget http://127.0.0.1:9090/test.log
```

##### 上传文件:
```shell
curl -X POST -F "file=@jquery-3.6.0.min.js" http://127.0.0.1:9090/test/test.log
```
