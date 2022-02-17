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
wget https://github.com/wanggaolin/go-fileHttp/archive/refs/tags/mac-v1.3.tar.gz
tar -xvf mac-v1.3.tar.gz
cd go-fileHttp-mac-v1.3   
./file_http
```

#### 默认配置
| Key               | Value              |Describe              |
|  ----------       | :-----------:      |   :-----------:      |                    
| ROOT_DIR          | $HOME              |   用户家目录           |
| ERROR_LOG         | error.log          |   日志                |
| ACCESS_LOG        | access.log         |   访问日志            |
| LISTEN            | 127.0.0.1:9191     |   监听地址             |
| PUSH              | true               |   允许上传             |
| SHOW_ALL          | false              |   显示隐藏文件或目录     |
| POSH_BACKUP       | false              |   上传时备份原有文件     |


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
