# Récupérer l'image Apache officielle.
FROM httpd:latest

# Nous place dans le dossier de travail du container.
WORKDIR /usr/local/apache2/htdocs/

# Copie le fichier index.html depuis TP_DOCKER_1 en local vers le dossier de travail du container précédemment définie.
COPY ./html/index.html .

# Mappe le port 80 sur Docker pour qu'il soit accessible depuis l'extérieur sur le port de l'hôte.
EXPOSE 80
