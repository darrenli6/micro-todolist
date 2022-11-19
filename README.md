# micro-todolist

## golang设置代理

https://developer.aliyun.com/article/879662


vim ~/.zshrc

export GOPATH=$HOME/go
export GOBIN=$GOPATH/bin
export PATH="$GOBIN:$PATH"



## 进入对应目录

`
protoc --proto_path=. --micro_out=. --go_out=. userModels.proto
`

- 忽略缓冲文件
`git rm -r --cached .idea `




 # error 

```azure

user imports
    github.com/micro/go-micro/v2/registry/etcd imports
        github.com/coreos/etcd/clientv3 tested by
        github.com/coreos/etcd/clientv3.test imports
        github.com/coreos/etcd/integration imports
        github.com/coreos/etcd/proxy/grpcproxy imports
        google.golang.org/grpc/naming: module google.golang.org/grpc@latest found (v1.51.0), but does not contain package google.golang.org/grpc/naming



go mod edit -replace google.golang.org/grpc@v1.51.0=google.golang.org/grpc@v1.29.1

```

