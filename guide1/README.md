



## Introduction




La réalité virtuelle a le potentiel de transformer l’éducation, en offrant des expériences d’apprentissage immersives et interactives. Les panoramas 360°, en particulier, peuvent permettre aux lycéens et étudiants de découvrir de nouveaux environnements et concepts d’une manière visuellement riche et engageante.




A-Frame, une bibliothèque JavaScript pour la création d’expériences de réalité virtuelle, rend cette technologie accessible à tous, même à ceux qui n’ont pas de connaissances approfondies en programmation. Avec A-Frame, vous pouvez consulter des panoramas 360° interactifs et immersifs directement dans votre navigateur web, ce qui est idéal pour une utilisation en classe ou à distance.




Sur cette page, nous vous guiderons à travers les étapes de la création de votre propre panorama 360° en utilisant A-Frame, spécifiquement adapté à un contexte éducatif. Nous commencerons par les bases, comme la configuration de votre environnement de développement et la prise de photos panoramiques, puis nous vous montrerons comment utiliser A-Frame pour assembler ces photos en une expérience de réalité virtuelle interactive.




Que vous soyez un enseignant cherchant à intégrer la réalité virtuelle dans votre salle de classe, un développeur web cherchant à créer des ressources éducatives interactives, ou simplement quelqu’un qui est curieux de la technologie de panorama 360°, nous espérons que vous trouverez cette page informative et utile. Bonne création !








# [Partie 1 - Matériel préparatoire et prises de vues](https://maximefr37.github.io/VR-Markdown/guide1/partie1/index.html)








## En amont : La planification




La planification, définissant l'objet de la visite et le contenu qui devra s'afficher, est essentielle en amont de toute production. Ceci est plus simple à dire qu'à faire, mais il est essentiel de définir l'objectif de la visite et d'avoir une idée claire de *ce qui doit être montré*.




Dans notre cadre, nous allons réaliser une visite virtuelle simple du terrain de sport de lycée Louis de Cormontaigne à Metz, se basant sur deux panoramas à 360°. Cette visite devra inclure des informations textuelles, des images, des vidéos, et des objets en 3 dimensions qui s'insèrent naturellement dans un panorama en 360°. Pour simplifier l'exemple, nous allons lier deux panoramas 360° entre eux pour permettre de simuler une ballade. Suivant la logique de navigation entre panoramas, l'orientation de l'utilisateur dans un panorama va avoir un impact: il est plus naturel quand on se déplace d'un point A à un point B que la vue lors de l'arrivée au point B suive une ligne droite issue du point A, afin de faire comprendre l'idée du mouvement. De même, l'ensemble des panoramas seront enrichis avec du contenu pédagogique sous diverses formes. Ce contenu doit s'afficher *à sa place* dans le panorama (par exemple le texte qui donne des informations sur un bâtiment doit flotter uniquement au-dessus de ce bâtiment).




Ceci explique l'importance d'une réflexion en amont, afin d'être sûr d'avoir toutes les images requises. Prendre une prise de vue manquante dans un deuxième temps risque expose l'opération à des changements brutaux de conditions de navigation (lumière ou météo différente par exemple) qui vont nuire à l'immersion.




Attention en particulier aux épineuses questions de droits à l'image et des conséquences potentielles au niveau du RGPD. Il peut être utile de demander aux personnes ne souhaitant pas être visibles sur le panorama de sortir du champ de la caméra.




## Matériel nécessaire




- Une caméra 360° (nous utiliserons une caméra Insta 360 pour cet exemple). 
- Un pied pour appareil photo (afin d'avoir une hauteur de prise de vue fixe entre les différents panoramas)
- Un ordinateur, avec les logiciels suivants
  - Un environnement de développement (ici [VSCodium](https://vscodium.com)
  - Un logiciel d'édition et de retouche d'image (ici [GIMP](https://gimp.org)
  - Un compte GitHub (nous utiliserons cette plateforme pour l'hébergement des scènes, et nous nous assurerons que vous puissiez retrouver les fichiers issus de ce document)








### Prise des vues 360°




Il est utile de bien planifier en amont de toutes prises de vues les endroits où seront réalisés les photos.
En extérieur, des outils comme Google Earth sont particulièrement utiles.




![planification](<partie2/resources/image/plan.jpg>)




L'importation des images est le moment idéal pour modifier la résolution en 2880 pixels par 1440 pixels avec le logiciel de la caméra. Pour flouter les visages (question de droits à l'image), nous allons utiliser GIMP.




## GIMP - un couteau suisse de l'image pour préparer les panoramas




GIMP est accessible gratuitement, ce qui en fait un outil économique pour les artistes et les créateurs. GIMP offre une gamme complète d'outils de retouche d'images, y compris des outils de peinture, de sélection, de correction des couleurs, de clonage, de transformation et bien d'autres encore. Cette diversité d'outils permet aux utilisateurs de réaliser une grande variété de tâches de retouche et de manipulation d'images, y compris la création de panoramas 360°.




### Importation des images




Importez toutes les images composant vos panoramas 360° dans GIMP au format JPEG et aux dimensions 2880 x 1440 pixels.




### Réglages et corrections




Effectuez des ajustements de couleur, de contraste et de netteté pour harmoniser les différents panoramas 360°. Vous pouvez également utiliser des outils de retouche pour éliminer les imperfections ou les éléments indésirables de certaines images.




### Exportation de panoramas




Une fois que votre panorama 360° est retouché, exportez-le dans le format JPEG, avec une qualité moyenne. Assurez-vous de choisir un format d'image compatible avec les plateformes ou les appareils sur lesquels vous prévoyez de partager votre panorama.
