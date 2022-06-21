```
#初始化operator
kubebuilder init --domain=lostar.cn --repo github.com/lostar01/app
kubebuilder create api --group app --version v1 --kind App --controller=true
```

```
#编译打包镜像
make help
make docker-build
```
