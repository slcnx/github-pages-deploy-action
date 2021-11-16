# github-pages-deploy-action
learn github action

# 构建代码并推送到dockerhub
在settings中配置secrets/environment，其中包含了认证dockerhub的token和用户名

在workflow中通过secrets context(会聚合所有的 repo/组织/environment的secret),来引用变量

通过docker 插件完成自动构建推送


只要push了就会执行

构建仓库主目录的Dockerfile

结果的镜像名是docker.io/slcnx/仓库名:分支名

