# 리포지토리 설명
- Jenkins Docker Out Of Docker 전략을 사용하기 위한 리포지토리
# How to Install?

```shell
git clone https://github.com/jimyungkoh/jenkins-docker.git
```

```shell
cd ./jenkins-docker
docker build -t jenkins-docker . 
```
# How to Run
```shell
docker run -p 80:8080 -p 50000:50000 -v /var/jenkins_home:/var/jenkins_home -v /var/run/docker.sock:/var/run/docker.sock --name j
enkins -d jenkins-docker
```