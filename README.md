# TP3: SPARK 
Veuillez procéder par $mvn package avant l'execution du code .
# Activité 2

Le fichier de données inputfile.txt est chargé dans HDFS <image1>.
On execute le code en Scala sur ce fichier inputfle.txt afin de compter le nombre d'occurences de chaque lettre dans ce dernier .

Voici la commande <image2> 

Le resultat est comme suit : 
<image3>

# Activité 3

On modifie le code en Scala pour afficher maintenant le nombre d'occurences de chaque mots dans le fichier de données .
<image4>
On execute SPARK et le resultat est comme suit :
<image5>

On procéde ensuite par la création du dossier MapReduce qui contient les codes du mapper et du reducer écrit en pyton pour executer la meme fonctionnalités .
Mapper:
<image6>
Reducer : 
<image7>

On lance le job Map Reudce comme suit :
<image8>

Le resultat : 
<image9>

La difference en temps d'execution n'est pas trés claire pour un fichier de données de petite taille qui nous a servi que pour le test .

Mais on executant ce comportement sur le fichier de données forun_nodes avec SPARK vs Map Reduce,on peut facilement affirmer que SPARK est plus rapide que Map reduce de hadoop .
En effet ,SPARK exploite efficacement la mémoire et rend l'execution de tel algorithme moins couteuse et plus efficae .
