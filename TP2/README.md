3.
- a. docker pull nginx
- b. docker image ls
- d. docker run -v C:\Users\YnovStudent\Desktop\x\Devops-Myriam\TP2\html:/usr/share/nginx/html -p 3000:80 nginx
- e. docker rm 86c9e508c544
- f. docker cp ./html 89g9e508c589:/usr/share/nginx/html

4.
- b. docker build C:\Users\YnovStudent\Desktop\x\Devops-Myriam\TP2\
- c. Le 4 est beaucoup plus rapide à exécuter, moins de commande et c'est automatisé.

5.
- a. docker pull mysql && docker pull phpmyadmin
- b.
 - 1. docker network mon-network
 - 2. docker run -d --name mysqldb --network mon-network -e MYSQL_ROOT_PASSWORD=mdp -p 3306:3306 mysql:latest
 - 3. docker run -d --name phpmyadmin --network mon-network -e PMA_HOST=mysqldb -e MYSQL_ROOT_PASSWORD=mdp -p 8080:80 phpmyadmin/phpmyadmin:latest

6.
- a. Faire plusieurs conteneurs et les configurer dans le meme fichier, aussi pour pour travailler ensemble
- b. docker-compose up
- b. docker-compose down