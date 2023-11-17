# kubernetes-gitlab
前置作業
1. 安裝 metalLB
2. 安裝 local-path  CSI

## 自建 gitlab 社群版

```
git clone https://github.com/cooloo9871/kubernetes-gitlab.git;cd kubernetes-gitlab/
```
```
$ kubectl create -f gitlab-ce/gitlab-ns.yml
```
```
$ kubectl create -f gitlab-ce/redis-svc.yml 
```
```
$ kubectl create -f gitlab-ce/redis-deployment.yml 
```
```
$ kubectl create -f gitlab-ce/postgresql-svc.yml 
```
```
$ kubectl create -f gitlab-ce/postgresql-deployment.yml
```
```
$ kubectl create -f gitlab-ce/gitlab-svc.yml 
```
```
$ kubectl create -f gitlab-ce/gitlab-svc-nodeport.yml 
```
```
$ kubectl create -f gitlab-ce/gitlab-deployment.yml
```

## 自建 gitlab 企業版

```
git clone https://github.com/cooloo9871/kubernetes-gitlab.git;cd kubernetes-gitlab/
```
```
kubectl apply -f gitlab-ee/gitlab-ee.yaml
```
