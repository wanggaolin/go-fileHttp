#### LANGUAGE
[中文](https://github.com/wanggaolin/go-fileHttp#readme)
[English](https://github.com/wanggaolin/go-fileHttp/blob/master/doc/readme_zh.md)

#### Describe
Lightweight file sharing system

![这是图片](doc/demo.png "Magic Gardens")

#### Install [for linux]
```shell
cd git clone https://github.com/wanggaolin/go-fileHttp.git && cd go-fileHttp && ./file_http 
```


#### default config 
| Key               | Value              |Describe              |
|  ----------       | :-----------:      |   :-----------:      |                    
| ROOT_DIR          | $HOME              |   User home directory           |
| ERROR_LOG         | error.log          |   error log                |
| ERROR_LOG         | access.log         |   access log               |
| LISTEN            | 0.0.0.0:9191       |   listen addres             |


### required parameter
| Header               | Value                           |Describe              |
|  ----------       | :-----------:                     |   :-----------:      |                    
| Content-Type      | application/json <br> application/text <br> application/html               |   请求返回类型          |


#### use/example
##### example1:
```shell
curl -H "Content-Type:application/json" http://127.0.0.1:9090/
curl -H "Content-Type:application/text" http://127.0.0.1:9090/
curl -H "Content-Type:application/text" http://127.0.0.1:9090/
```
