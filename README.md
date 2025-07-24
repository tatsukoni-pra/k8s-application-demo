# k8s-application-demo

## ビルドコマンド

```
$ cd docker
$ aws ecr get-login-password --region ap-northeast-1 --profile tatsukoni | docker login --username AWS --password-stdin 083636136646.dkr.ecr.ap-northeast-1.amazonaws.com
$ docker build -t k8s-application-nginx .
$ docker tag k8s-application-nginx:latest 083636136646.dkr.ecr.ap-northeast-1.amazonaws.com/k8s-application-nginx:20250725v1
$ docker push 083636136646.dkr.ecr.ap-northeast-1.amazonaws.com/k8s-application-nginx:20250725v1
```
