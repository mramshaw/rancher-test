# rancher-test

Getting familiar with Rancher

## Motivation

[Rancher](http://rancher.com/) offers a nice GUI for Multi-Cluster Kubernetes Management.

This is an option for anyone who does not with to use `helm`.

Of course, under the covers Rancher actually uses `helm` itself, but sometimes a dashboard is handy.

Rancher also offers a CLI tool.

## Run with Docker

```bash
$ docker run --name helm_rancher --restart=unless-stopped -p 80:80 -p 443:443 rancher/rancher
Unable to find image 'rancher/rancher:latest' locally
latest: Pulling from rancher/rancher
6cf436f81810: Pull complete 
987088a85b96: Pull complete 
b4624b3efe06: Pull complete 
d42beb8ded59: Pull complete 
20428076f45c: Pull complete 
aa5f6ec4068f: Pull complete 
fa0b81e2aefe: Pull complete 
174adca119fa: Pull complete 
b36e95625791: Pull complete 
3b4599da8bc5: Pull complete 
7c3eae4ec924: Pull complete 
821c0eae95fd: Pull complete 
Digest: sha256:1943e9b7d802992d3c61184af7ae2ca5d414c15152bc40ec995e71e28cb80844
Status: Downloaded newer image for rancher/rancher:latest
52c9be72fb2c6a7c7ff7a877be39a828ed36412ba1a2d58395bb4608b6f1add0
$
```

[My usual practice is to specify a version for Docker images; here we are evaluating
 Rancher - so we defintely want the ___latest___ version.]

## User Interface

Helm offers a nice dark theme:

![Helm dark](images/Rancher_dark_theme.png)

## Versions

* Docker (Client and Server) - __18.09.3__
* kubectl __v1.10.7__
* Kubernetes __v1.13.4__
* minikube __v0.35.0__
* Rancher
* virtualbox __5.1.38__
