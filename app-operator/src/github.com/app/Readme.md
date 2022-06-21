``
我们将定义一个 crd ，spec 包含以下信息：

Replicas	# 副本数
Image		# 镜像
Resources	# 资源限制
Envs		# 环境变量
Ports		# 服务端口
``

``
#初始化operator
kubebuilder init --domain=lostar.cn --repo github.com/lostar01/app
kubebuilder create api --group app --version v1 --kind App --controller=true
``

``
#编译打包镜像
make help
make docker-build
``
