### virtualisation : abstraction du hardware || virtualisation software :=> container 
### namespaces alloues ressources à une seul processus avec cgroup on peut mettre limitation des ressources ces composant que docker l'utilise pour partage les ressources entre les host et les containers => docker il ajout des couches d'abstraction.
### VMS sont des maisons , les containers sont des chambres.
### image (r-o) ,container (r-w)
### le minimuim os ubuntu 18.04
### executer commande dans un container
```bash
docker run busybox /bin/sh -c 'echo $(date)'
```
### execute multiple commande *
```bash
docker run -it busybox /bin/sh 
```
### voir container en cours
```bash
docker ps
```
### or 
```bash
docker container list || ls
```

### voir container en arret
```bash
docker container list || ls -a 
```
### other workshop in link bellow
```bash
https://gist.github.com/med363/62e2226c3eb8cdf8cd7d66aa3d4931cf
```
### voir web ser in terminal je peut install elinks
```bash
apt install elinks
```
et on tappe 
```bash
elinks  @ip
```
### volumes par defauts sur /var/lib/docker/volumes/
```bash
docker volume create --name maria_data
```
### other article for network 
```bash
https://devopssec.fr/article/fonctionnement-manipulation-reseau-docker
```


 


