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

d. Démarrer un nouveau container et servir la page html créée précédemment à l'aide d'une référence absolue (chemin de racine à racine):

```bash
docker run -dp 8080:80 --name contenair_index.html -v D:\Git\TP_DOCKER\TP_DOCKER_1\html\index.html:/usr/local/apache2/htdocs/index.html  httpd:latest
docker ps
```
- Res : e2647ed9fff8   httpd:latest   "httpd-foreground"   10 seconds ago   Up 3 seconds   0.0.0.0:8080->80/tcp   contenair_index.html
