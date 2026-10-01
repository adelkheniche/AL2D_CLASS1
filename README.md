# Awesome dessin vectoriel & fabrication 2D

Une liste de ressources pour comprendre le dessin vectoriel et découvrir les possibilités du laser, de la découpe vinyle et du fraisage CNC.

**Bachelor Human IT · ENSEA · Première année**

**Logiciel utilisé pendant le cours : Affinity Designer.**

## Sommaire

* [Comprendre le dessin vectoriel](#comprendre-le-dessin-vectoriel)
* [Découper et graver au laser](#découper-et-graver-au-laser)
* [Découper du vinyle et imprimer des motifs](#découper-du-vinyle-et-imprimer-des-motifs)
* [Fraiser et changer d’échelle](#fraiser-et-changer-déchelle)
* [Dessin et préparation des fichiers](#dessin-et-préparation-des-fichiers)
* [Source](#source)

## Comprendre le dessin vectoriel

* **Raster ou vectoriel** — [Comparaison visuelle](assets/raster-vectoriel.png)  
  *Une image raster contient une grille de pixels et leurs couleurs. Un dessin vectoriel contient des objets géométriques : un cercle possède un centre et un rayon, un chemin relie des points par des segments ou des courbes.*

* **Agrandir une image ou une forme** — [Comparaison raster / vectoriel](assets/raster-vectoriel.png)  
  *Agrandir un PNG conserve sa grille de pixels : on finit par voir des carrés ou du flou. Agrandir un objet vectoriel conserve sa définition géométrique. L’écran affiche finalement les deux avec des pixels.*

* **Nœuds, chemins et courbes de Bézier** — [Schéma d’une courbe](assets/bezier.png) · [Outil Nœud — Affinity Designer](https://affinity.help/designer2/fr.lproj/pages/Tools/tools_node.html) · [SVG à manipuler](exemples/demo-vectoriel.svg)  
  *Les nœuds placent les points du chemin. Les poignées règlent sa direction et sa courbure. Déplacer une poignée change la forme sans repeindre des pixels. Le dessin vectoriel est une description géométrique, pas simplement une collection de flèches mathématiques.*

* **Apprendre à utiliser la Plume** — [The Bézier Game](https://bezier.method.ac/) · [Outil Plume — Affinity Designer](https://affinity.help/designer2/fr.lproj/pages/Tools/tools_pen.html)  
  *Un exercice interactif pour apprendre à placer les nœuds et orienter les poignées afin de reproduire un tracé. À faire avant de dessiner avec la Plume dans Affinity Designer : on retrouve les mêmes principes de construction des courbes.*

* **Contour et remplissage** — [Trois opérations laser](assets/operations.png)  
  *Un contour peut être découpé ou marqué. Un disque vectoriel rempli peut être gravé par balayage. Le type de dessin et le mode de fabrication sont deux choix distincts.*

* **Une photo imprimée, un contour découpé** — [Print & cut — Roland DG](https://www.rolanddga.com/en-la/products/printers/versastudio-bn-20-t-shirt-printing-press)  
  *Une photo raster peut être imprimée ou gravée telle quelle. Pour découper son pourtour, on ajoute un contour vectoriel. Un document peut contenir les deux.*

* **Vectoriser une image** — [Redessiner avec la Plume — Affinity Designer](https://affinity.help/designer2/fr.lproj/pages/Tools/tools_pen.html)  
  *Vectoriser reconstruit des chemins à partir des pixels. Enregistrer une photo dans un SVG ne suffit pas. Le résultat demande souvent du nettoyage pour obtenir des contours précis.*

## Découper et graver au laser

* **Motifs et répétitions** — [Cuttle, éditeur vectoriel et motifs paramétriques](https://cuttle.xyz/)  
  *Une forme élémentaire peut produire un motif entier. Application : un panneau ajouré ou une grille de ventilation.*

* **Marqueterie et incrustations** — [Incrustation de guitare, Epilog](https://www.epiloglaser.com/fr/ressources/club-d-echantillons/decoupe-au-laser-d-une-incrustation-de-guitare/)  
  *Les contours donnent des pièces qui se complètent. La précision d’ajustement compte autant que le motif.*

* **Boîtes et boîtiers** — [ElectronicsBox, Boxes.py](https://boxes.hackerspace-bamberg.de/ElectronicsBox?language=en)  
  *Le volume vient de l’assemblage. Modifier largeur, hauteur ou épaisseur change les contours générés.*

* **Living hinges : charnières souples** — [Living hinges, exemples MIT](https://academy.cba.mit.edu/classes/computer_cutting/hinges.jpg) · [FlexBox, générateur Boxes.py](https://boxes.hackerspace-bamberg.de/FlexBox?language=en)  
  *Un dessin change la souplesse de la pièce. Le résultat dépend de la matière et du motif.*

* **Cuir : découpe et décoration** — [Portefeuilles en cuir, Epilog](https://www.epiloglaser.com/fr/ressources/club-d-echantillons/portefeuilles-en-cuir-grave-decoupe-au-laser/)  
  *Coupe et gravure remplissent des fonctions différentes. Utiliser uniquement un cuir validé pour le laser du lab.*

* **PMMA : signalétique et lumière** — [Enseigne en acrylique et contreplaqué éclairée par LED, Epilog](https://www.epiloglaser.com/fr/ressources/club-d-echantillons/enseigne-led-en-acrylique-grave-au-laser/)  
  *Découper définit la silhouette ; graver produit un effet de surface. Exemple pour associer fabrication 2D et électronique.*

* **Des couches qui deviennent un relief** — [Ornements en bois multicouches, Epilog](https://www.epiloglaser.com/fr/ressources/club-d-echantillons/ornements-en-bois-multicouches-decoupes-au-laser/)  
  *L’empilement donne de la profondeur sans usiner une surface 3D.*

* **Des pièces planes qui deviennent une lampe** — [Lampe en bois découpée au laser, Epilog](https://www.epiloglaser.com/fr/ressources/club-d-echantillons/lampe-en-bois-decoupee-au-laser/)  
  *Le dessin prépare aussi les connexions entre les pièces.*

* **Des mécanismes et des pièces mobiles** — [Linkage, générateur de biellettes Boxes.py](https://boxes.hackerspace-bamberg.de/Linkage?language=en) · [Flexures, exemples MIT](https://academy.cba.mit.edu/classes/computer_cutting/flexures.png)  
  *On peut fabriquer une géométrie qui bouge. Un mécanisme demande des jeux et parfois des éléments ajoutés.*

* **Papier, kirigami et déploiement** — [Origami Simulator, Amanda Ghassaei](https://origamisimulator.org/)  
  *Un plan peut décrire un objet déployable. La simulation montre le pliage ; la coupe et les éventuels plis doivent ensuite être préparés pour la machine disponible.*

* **Une image gravée** — [Exemple de gravure raster présenté au MIT](https://academy.cba.mit.edu/classes/computer_cutting/raster.jpg)  
  *La photographie peut rester raster. Sa gravure n’exige pas de reconstruire tous ses détails en chemins.*

* **Pour ouvrir les possibilités : LaserOrigami** — [LaserOrigami, projet de recherche de Stefanie Mueller, Bastian Kruck et Patrick Baudisch](https://hcie.csail.mit.edu/research/laserorigami/laserorigami.html)  
  *La recherche peut combiner découpe et déformation. Ce procédé spécifique nécessite une configuration adaptée ; il ne décrit pas une fonction prête à utiliser sur le laser du lab.*

## Découper du vinyle et imprimer des motifs

* **Lettres, pictogrammes et signalétique** — [Applications de découpe vinyle, cours MIT](https://academy.cba.mit.edu/classes/computer_cutting/index.html)  
  *La lame suit les contours, puis on retire les parties inutiles : c’est l’échenillage. Le film permet de transférer plusieurs éléments en conservant leur position.*

* **Motifs sur textile** — [Applications de transfert textile, Roland DG](https://www.rolanddga.com/en-la/products/printers/versastudio-bn-20-t-shirt-printing-press) · [![Motif appliqué sur textile par transfert](https://image.rolanddga.com/-/media/roland/images/products/printers/bn20-series/applications/heat-transfer-graphic.jpg?rev=38af29aafb3042a7a45073cf07046e63)  
  *Un film adapté permet de transférer un dessin sur un textile avec une presse. Le sens du dessin, les étapes et les réglages dépendent du film utilisé. Photo : **Roland DG**.*

* **Print & cut : photo imprimée, contour découpé** — [BN-20A, impression et découpe de contours, Roland DG](https://www.rolanddga.com/en-la/products/printers/versastudio-bn-20-t-shirt-printing-press)  
  *Le contenu imprimé peut mêler photos et vectoriel. Le contour commande la découpe. C’est le meilleur exemple pour comprendre pourquoi on peut avoir les deux dans un seul fichier.*

* **Pochoirs et masques** — [Applications de masquage et sérigraphie, MIT](https://academy.cba.mit.edu/classes/computer_cutting/index.html)  
  *Le centre d’un O doit rester attaché par des ponts si le pochoir est d’un seul tenant. Le dessin doit tenir compte de l’objet final.*

* **Circuits souples et antennes** — [Expérimentations de Jie Qi : électronique et matériaux souples](https://fab.cba.mit.edu/classes/863.10/people/jie.qi/jieweek10.html)  
  *Un contour peut aussi définir une piste conductrice. Cette piste d’exploration demande un matériau, une lame et une procédure compatibles ; elle n’est pas une capacité confirmée de toutes les découpeuses.*

## Fraiser et changer d’échelle

Les lasers et les découpeuses vinyle sont aussi des machines à commande numérique. Ici, « CNC » désigne le fraisage.

* **Mobilier à assembler** — [Exemples de mobilier fabriqué par CNC, ShopBot](https://shopbottools.com/applications/furniture/)  
  *On retrouve la logique des boîtes, à une autre échelle. Une fraise ronde laisse des angles intérieurs arrondis ; les assemblages peuvent demander des dégagements de type dogbone.*

* **Une poche pour loger une pièce** — [Poche, coupe intérieure et coupe extérieure : guide Nomad 3, Carbide 3D](https://my.carbide3d.com/pdf/Nomad3_Getting_Started_Guide_12_22_2020_v1_smaller.pdf)  
  *Le même dessin 2D peut conduire à une découpe traversante ou à un creux. Il faut ajouter profondeur et diamètre d’outil dans la préparation des parcours.*

* **Une zone fermée pour usiner une poche** — [Pocketing out an area, tutoriel de William Adams, Carbide 3D](https://community.carbide3d.com/t/pocketing-out-an-area/80732)  
  *Un contour qui semble correct à l’écran peut avoir une ouverture. La fabrication rend visibles ces erreurs.*

* **Construction à partir de panneaux** — [WikiHouse, système constructif](https://www.wikihouse.cc/)  
  *On peut passer du contour d’une pièce à un système de construction. Un bâtiment exige une conception et une validation structurelle spécifiques.*

* **Pour distinguer 2D et relief 3D** — [Mobilier topographique de Sam Sheckells, ShopBot](https://shopbottools.com/2025/10/09/sam-sheckells-puts-a-topographic-twist-on-furniture/)  
  *Des contours et des profondeurs suffisent à certaines opérations 2,5D. Une surface de relief continu nécessite une représentation 3D et des parcours adaptés.*

## Dessin et préparation des fichiers

* **Dessiner dans Affinity Designer** — [Outil Plume — Affinity Designer](https://affinity.help/designer2/fr.lproj/pages/Tools/tools_pen.html) · [Outil Nœud — Affinity Designer](https://affinity.help/designer2/fr.lproj/pages/Tools/tools_node.html) · [Fichier de démonstration](exemples/demo-vectoriel.svg)  
  *Premier objectif : dessiner une forme à la bonne dimension, modifier ses nœuds et soustraire une forme à une autre. Le cours utilise uniquement Affinity Designer.*

* **Formats SVG, PDF, DXF et images raster** — [Exemple de fichier SVG](exemples/demo-vectoriel.svg)  
  *PNG et JPEG contiennent des pixels. SVG et PDF peuvent mêler vectoriel et raster. Le DXF sert à échanger de la géométrie CAO. Vérifier le contenu, les unités et les dimensions après chaque import.*

* **Texte et courbes** — [Convertir des objets en courbes — Affinity Designer](https://affinity.help/designer2/fr.lproj/pages/ObjectControl/converttocurves.html)  
  *Convertir le texte en courbes lorsque le workflow le demande évite de dépendre d’une police absente. Conserver aussi une version éditable du document.*

* **Générer plutôt que tout redessiner** — [Boxes.py](https://boxes.hackerspace-bamberg.de/) · [Cuttle](https://cuttle.xyz/)  
  *Un générateur produit des contours à partir de paramètres. Comprendre ses dimensions et ses réglages reste nécessaire pour adapter le résultat à la matière et à l’usage.*

* **Largeur de coupe et jeu d’assemblage** — [Kerf et assemblages — MIT](https://academy.cba.mit.edu/classes/computer_cutting/index.html) · [Boîtiers paramétriques — Boxes.py](https://boxes.hackerspace-bamberg.de/ElectronicsBox?language=en)  
  *Le laser enlève une petite largeur de matière. Deux pièces dessinées à la même cote ne s’emboîtent pas forcément. Mesurer l’épaisseur réelle et tester l’ajustement avant de fabriquer l’ensemble.*

* **Contours fermés et doublons** — [Régions fermées — Carbide 3D](https://community.carbide3d.com/t/pocketing-out-an-area/80732)  
  *Fermer les contours nécessaires, supprimer les lignes superposées et vérifier les éléments isolés. Une erreur discrète à l’écran peut produire une coupe répétée ou empêcher une opération.*

* **Organiser les pièces sur la plaque** — [Deepnest](https://deepnest.io/)  
  *L’imbrication des pièces réduit les chutes. Prévoir aussi les contraintes de matière et l’espacement entre pièces.*

* **Du dessin aux mouvements de l’outil** — [Laser et découpe à lame — MIT](https://academy.cba.mit.edu/classes/computer_cutting/index.html) · [FAO et fraisage — MIT](https://academy.cba.mit.edu/classes/computer_machining/index.html)  
  *Le dessin décrit la géométrie. Le logiciel de fabrication ajoute les opérations et les réglages. Une couleur rouge ou un trait épais n’a pas de signification machine universelle.*

* **Matière et sécurité** — [Sécurité et matériaux — MIT](https://academy.cba.mit.edu/classes/computer_cutting/index.html)  
  *Utiliser les matériaux validés pour la machine du lab. Un vinyle peut contenir du PVC : il reste destiné à la lame et ne passe pas au laser. Les épaisseurs de l’ancien support ne constituent pas des limites universelles.*

## Source

* [Computer-Controlled Cutting — Neil Gershenfeld, MIT Center for Bits and Atoms](https://academy.cba.mit.edu/classes/computer_cutting/index.html) · [Computer-Controlled Machining — MIT](https://academy.cba.mit.edu/classes/computer_machining/index.html)  
  *Liste adaptée à une découverte de 30 minutes, à partir du support « Initiation LASER 1.0.1 » d’Adel Kheniche : motifs, marqueterie, boîtes, charnières souples, cuir, PMMA et gravure. Format repris du dépôt AL3D_CLASS-.*
