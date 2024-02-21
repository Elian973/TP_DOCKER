# TP1 DOCKER

## 2 . Dans un repo GIT&GithuB, créez un dossier TP_DOCKER_1

## 3 . Executer un serveur web (apache) dans un container docker

a. Récuperer l'image sur le docker hub (httpd)

```bash
docker pull httpd:latest
```

b. Vérifier que vous disposez bien de l'image en local

```bash
docker images
```
- Res: httpd        latest    2776f4da9d55   5 weeks ago   167MB

c. Créer un fichier ./html/index.html

```bash
mkdir ./html
echo "Hello World" > ./html/index.html
```

d. 