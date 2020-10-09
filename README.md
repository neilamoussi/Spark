# SPARK 
Veuillez procéder par $mvn package avant l'execution du code .
# Activité 2

Le fichier de données inputfile.txt est chargé dans HDFS ![1](https://cloud.githubusercontent.com/assets/16022349/25381382/cb0478b0-29b3-11e7-8be9-fb8de1c7e8b3.png).
On execute le code en Scala sur ce fichier inputfle.txt afin de compter le nombre d'occurences de chaque lettre dans ce dernier .

Voici la commande ![2](https://cloud.githubusercontent.com/assets/16022349/25381403/df4d0c10-29b3-11e7-8620-d2f040532002.png)

Le resultat est comme suit : 
![3](https://cloud.githubusercontent.com/assets/16022349/25381413/eee20824-29b3-11e7-862b-967ecd2e57ae.png)

# Activité 3

On modifie le code en Scala pour afficher maintenant le nombre d'occurences de chaque mots dans le fichier de données .
![4](https://cloud.githubusercontent.com/assets/16022349/25381421/fd50f636-29b3-11e7-9008-5156730aba4a.png)
On execute SPARK et le resultat est comme suit :
![5](https://cloud.githubusercontent.com/assets/16022349/25381438/0d888bea-29b4-11e7-9e77-2466f0036500.png)

On procéde ensuite par la création du dossier MapReduce qui contient les codes du mapper et du reducer écrit en pyton pour executer la meme fonctionnalités .
Mapper:
![6](https://cloud.githubusercontent.com/assets/16022349/25381464/2b28a7de-29b4-11e7-9d50-6a5ab5781c2d.png)
Reducer : 
![7](https://cloud.githubusercontent.com/assets/16022349/25381474/3535e5a2-29b4-11e7-98a9-8d8503fb7b92.png)

On lance le job Map Reudce comme suit :
![8](https://cloud.githubusercontent.com/assets/16022349/25381493/490e524e-29b4-11e7-945c-0eeaace34430.png)

Le resultat : 
![9](https://cloud.githubusercontent.com/assets/16022349/25381801/6fef52c2-29b5-11e7-935a-17bb77150fc2.png)


La difference en temps d'execution n'est pas trés claire pour un fichier de données de petite taille qui nous a servi que pour le test .

Mais on executant ce comportement sur le fichier de données forun_nodes avec SPARK vs Map Reduce,on peut facilement affirmer que SPARK est plus rapide que Map reduce de hadoop .
En effet ,SPARK exploite efficacement la mémoire et rend l'execution de tel algorithme moins couteuse et plus efficae .
