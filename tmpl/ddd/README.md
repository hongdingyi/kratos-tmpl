# kratos-ddd

尝试使用kratos，采用DDD 项目风格

# 启动命令：
 当前采用etcd做服务发现
./kratos-ddd -conf ../configs/ -appid kratos-ddd -discovery.nodes 127.0.0.1:2379

# proto 生成工具
[prototool](https://github.com/mfslog/prototool)

# 接口测试

接口测试工具采用[grpcui](https://github.com/fullstorydev/grpcui)

参考命令：

在项目目录下执行：

grpcui -plaintext -import-path . -import-path $GOPATH/src/github.com/bilibili/kratos/third_party  -proto kratos.proto -port 8080 localhost:9000

# 参考
[dotnet-architecture / eShopOnContainers](https://github.com/dotnet-architecture/eShopOnContainers)

[alibaba/COLA](https://github.com/alibaba/COLA)