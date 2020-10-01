# Symfony 4.4

## Pour commencer

Docker pour une application Symfony 4.4 avec quelques dépendances: 

 * Apache
 * Mysql 8
 * Php 7.2.3
 * PhpMyAdmin

### Conditions préalables


Pour faire fonctionner ce conteneur, vous devez installer docker.

* [Windows](https://docs.docker.com/windows/started)
* [OS X](https://docs.docker.com/mac/started/)
* [Linux](https://docs.docker.com/linux/started/)

### Build

1. Cloner le repo

        git clone https://github.com/Valharault/TPGit.git
        
2. Installer le package

        cd TPGit
        docker-compose up -d
        docker-compose exec php bash -c "cd sf4;composer install"

    Cela prendra quelques minutes.

3. Lancer le service

        docker-compose up -d
        Le flag -d permet de détacher le service
        
4. Commandes utiles
        
        Arrêter le service 
        $ docker-compose stop 
        Lancer le service 
        $ docker-compose up -d

6. Une fois que tout a démarré, vous devriez pouvoir accéder à la webapp via [http://localhost/](http://localhost/) sur votre machine hôte.

        open http://localhost/

