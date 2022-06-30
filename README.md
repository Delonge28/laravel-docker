
# Rejoose docker on azure

A step by step to deploy an application with docker on Azure
## Steps to deploy an App using docker on azure



```bash
  Create Container registry on azure
```

```bash
  Create Dockerfile locally
```

```bash
  Build Dockerfile – docker build -t <name> . 
```
---- To run locally – docker run -p 8888:80 <name> 

```bash
  Login to azure via termial – az login. (make sure you have Azure CLI)
```



```bash
  Login to registry – az acr login --name <registryname>
```

```bash
  Docker tag <name> <dockerregistry>.azurecr.io/<name>
```

```bash
  Docker push <dockerregistry>.azurecr.io/<name>
```
