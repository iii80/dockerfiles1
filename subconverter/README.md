# subconverter

GitHub [stilleshan/dockerfiles](https://github.com/stilleshan/dockerfiles)  
Docker [stilleshan/subconverter](https://hub.docker.com/r/stilleshan/subconverter)
> *docker image support for X86 and ARM*

## 简介
基于 [tindy2013/subconverter](https://github.com/tindy2013/subconverter) 项目的 docker 镜像.仅修改 **分组配置文件** 以解决以下问题.

- **增加**`Netflix`分组
- **去除**`自动选择 url-test`以解决连接数爆涨问题.
- **全球拦截** 增加`节点选择`,以满足`Google Analytics`等广告统计工具的访问需求.(新版本可能已解决此需求)
- **修改时区** 镜像默认时区为 Asia/Shanghai

## 更新
**2021-06-09** 更新`v0.6.4`版 docker 镜像,新增同时支持 X86 和 ARM 架构.

## 部署
### docker
```shell
docker run  -d --name=subconverter --restart=always -p 25500:25500 stilleshan/subconverter
```

### docker compose
下载 [docker-compose.yml](https://raw.githubusercontent.com/stilleshan/dockerfiles/main/subconverter/docker-compose.yml) 执行以下命令启动:
```shell
docker-compose up -d
```


## 使用
### 网友分享的订阅转换地址
> https://sub.ops.ci  
https://subto.herokuapp.com


## 参考
GitHub [tindy2013/subconverter](https://github.com/tindy2013/subconverter)
