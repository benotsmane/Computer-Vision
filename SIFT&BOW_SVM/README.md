Nous allons preparer le developpement d’un premier modèle de classification d’images. L’objectif est de produire un algorithme capable de classer les images du jeu de donnees 15-Scenes, qui contient 4485 images appartenant à 15 catégories de scènes intérieures et extérieurs (cuisine, chambre,rue,etc.)

Pour cela, nous allons dans un premier temps utiliser des **SIFT**(Scale-invariant featuretransform), qui est un descripteur visuel local et qui permet donc de caracteriser numériquement un petit patch d’image. On cherchera ensuite des descripteurs-types représentant des motifs fréquents parmi tous les SIFT de notre jeu  d’images pour constituer un dictionnaire visuel. Puis, on aggrégera les SIFT de chaque image avec la technique du **BoW**(Bag of Words) qui permet de représenter numériquement et de maniére condensée une image.

On apprendra à classer chaque image à partir de sa représentation condensée à l’aide d’un **SVM**(Support Vector Machine).
