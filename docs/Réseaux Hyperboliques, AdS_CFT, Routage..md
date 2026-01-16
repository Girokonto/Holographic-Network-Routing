# **Isomorphisme Holographique : Correspondances Théoriques entre le Routage Géométrique Hyperbolique dans les Réseaux Complexes et la Dualité AdS/CFT**

## **Résumé Exécutif**

Ce rapport de recherche exhaustif explore les correspondances structurelles, dynamiques et informationnelles entre la géométrie des réseaux complexes (tels que l'Internet, les réseaux sociaux et les connectomes biologiques) et la dualité Anti-de Sitter/Conformal Field Theory (AdS/CFT), également connue sous le nom de Principe Holographique. S'appuyant sur les travaux fondateurs de Dmitri Krioukov, M. Ángeles Serrano et Marián Boguñá, cette analyse postule que l'émergence des propriétés topologiques universelles des réseaux complexes — distribution des degrés en loi de puissance, fort coefficient de clustering et propriété de "petit monde" — n'est pas le fruit du hasard, mais la projection discrète d'une géométrie hyperbolique latente à courbure négative constante.

L'étude s'inscrit dans le contexte du modèle **TPDBT** (Topologie-Physique-Données-Bande passante-Tenseur), un cadre intégrateur qui encode les décisions de routage via des coordonnées virtuelles dans un "bulk" hyperbolique. Nous démontrons que l'efficacité du routage glouton ("greedy routing") dans ces réseaux est isomorphe au comportement des géodésiques dans un espace-temps AdS. De plus, nous examinons les implications profondes de la formule de Ryu-Takayanagi, interprétant le théorème "min-cut/max-flow" de la théorie des graphes comme un duel classique de l'entropie d'intrication holographique, fournissant ainsi une borne théorique à la capacité de transport d'information. L'analyse s'étend aux réseaux de tenseurs, spécifiquement l'Ansatz de Renormalisation de l'Intrication Multi-échelle (MERA), identifié comme l'architecture discrète reliant le bord (le réseau observable) et le bulk (le flux de renormalisation). Enfin, nous évaluons l'hypothèse de "Cosmologie Réticulaire", selon laquelle la dynamique de croissance des réseaux complexes reflète la structure causale d'un univers en accélération (de Sitter).

## ---

**Chapitre 1 : Introduction et Changement de Paradigme Géométrique**

### **1.1 La Crise de la Topologie et l'Hypothèse de la Géométrie Latente**

La science des réseaux, depuis ses débuts formels à la fin du XXe siècle, s'est principalement concentrée sur la caractérisation statistique des graphes. Les modèles classiques, tels que les graphes aléatoires d'Erdős-Rényi ou le modèle de configuration, ont échoué à capturer simultanément les trois propriétés ubiquistes des réseaux réels : l'hétérogénéité des degrés (souvent décrite par des distributions sans échelle ![][image1]), le fort clustering (tendance à la transitivité des connexions) et la faible distance moyenne entre les nœuds (effet "petit monde"). Pendant longtemps, ces propriétés ont été traitées comme des artefacts séparés, nécessitant des mécanismes génératifs ad hoc comme l'attachement préférentiel de Barabási-Albert pour l'hétérogénéité, ou le modèle de Watts-Strogatz pour le clustering.

Cependant, un changement de paradigme fondamental a été initié par les travaux de Dmitri Krioukov et de ses collaborateurs.1 Leur hypothèse centrale, souvent qualifiée d'hypothèse de la **géométrie latente**, postule que la topologie observable d'un réseau complexe n'est que l'ombre portée d'une structure métrique sous-jacente. Selon cette vision, les nœuds du réseau existent dans un espace métrique caché, et la probabilité de connexion entre deux nœuds dépend de leur distance dans cet espace.

L'intuition clé réside dans la nature de cet espace caché. Si l'espace était euclidien (plat), l'expansion du volume avec le rayon serait polynomiale (![][image2]), ce qui est insuffisant pour accommoder l'expansion exponentielle des nœuds observée dans les réseaux hiérarchiques et sans échelle. En revanche, dans une géométrie à courbure négative constante (géométrie hyperbolique), le volume de l'espace croît exponentiellement avec le rayon (![][image3]). Cette propriété d'expansion exponentielle est isomorphe à la structure arborescente (ou dendrogramme) qui caractérise les taxonomies hiérarchiques des systèmes complexes. Ainsi, l'hypothèse de Krioukov suggère que les réseaux complexes sont des discrétisations de la géométrie hyperbolique.3

### **1.2 Le Contexte TPDBT : Une Architecture Unifiée**

Afin de structurer cette analyse théorique, nous adoptons le cadre conceptuel **TPDBT**, qui permet de décomposer la problématique du routage holographique en cinq dimensions interdépendantes :

1. **Topologie (T) :** Le réseau observable, constitué de nœuds et de liens, qui réside sur le "bord" de l'espace géométrique.  
2. **Physique (P) :** Les lois statistiques régissant la probabilité de connexion, spécifiquement l'application de la statistique de Fermi-Dirac aux distances hyperboliques, traitant les liens comme des fermions non-interagissants.  
3. **Données (D) :** Les flux d'information qui doivent naviguer dans cette structure, soumis aux contraintes de localité et de causalité imposées par la géométrie.  
4. **Bande Passante (B) :** La capacité du réseau, analysée à travers le prisme de l'entropie d'intrication et des goulots d'étranglement géométriques (surfaces minimales).  
5. **Tenseur (T) :** La représentation discrète de l'espace latent via des réseaux de tenseurs hiérarchiques comme MERA, offrant un substrat computationnel pour la renormalisation.

Ce rapport défend la thèse que le "Routage Holographique" n'est pas simplement une métaphore poétique, mais une description mathématique rigoureuse où le chemin optimal pour le flux d'information dans un réseau invariant d'échelle suit une trajectoire à travers le "bulk" hyperbolique. Cette trajectoire exploite la hiérarchie du réseau pour minimiser la distance effective, un processus analogue au voyage des particules dans un espace-temps courbe décrit par la correspondance AdS/CFT.

### **1.3 Convergence Interdisciplinaire**

Notre analyse se situe au carrefour de trois disciplines majeures dont la convergence récente offre des perspectives inédites :

* **Physique Théorique des Hautes Énergies :** Spécifiquement la dualité AdS/CFT, qui relie une théorie gravitationnelle dans un volume (bulk) à une théorie quantique des champs sur sa surface (bord).  
* **Science des Réseaux et des Systèmes Complexes :** L'étude de la navigabilité, de l'auto-similarité et des processus de transport dans des graphes massifs.  
* **Théorie de l'Information Quantique :** L'utilisation de l'entropie d'intrication et des réseaux de tenseurs pour caractériser les corrélations dans les systèmes à N corps.

L'objectif est de démontrer que les défis de "navigabilité" rencontrés par l'Internet ou le cerveau humain sont résolus par l'adoption spontanée d'une architecture hyperbolique, la même architecture que l'univers semble adopter pour coder l'information gravitationnelle.

## ---

**Chapitre 2 : Fondements Théoriques de la Géométrie Hyperbolique des Réseaux**

### **2.1 Le Modèle du Disque de Poincaré et la Carte ![][image4]**

Pour comprendre l'isomorphisme proposé, il est impératif de définir le substrat géométrique. Le modèle standard employé dans la littérature est la représentation du disque de Poincaré de l'espace hyperbolique à deux dimensions (![][image4]). Dans ce modèle, l'intégralité du plan hyperbolique infini est projetée à l'intérieur d'un disque euclidien unitaire de rayon ![][image5].1

La métrique de cet espace diffère radicalement de l'intuition euclidienne. La distance hyperbolique ![][image6] entre deux points de coordonnées polaires ![][image7] et ![][image8] est donnée par la loi des cosinus hyperbolique :

![][image9]  
Pour des rayons ![][image10] suffisamment grands (ce qui est le cas pour la majorité des nœuds situés près du bord du disque), cette distance peut être approximée par :

![][image11]  
Cette équation révèle une propriété cruciale : la distance est la somme des coordonnées radiales plus un terme logarithmique dépendant de la séparation angulaire. Cela implique que pour minimiser la distance ![][image6] entre deux points éloignés angulairement, il faut passer par le centre du disque (où ![][image12] est petit), plutôt que de longer le bord.4

### **2.2 L'Interprétation Sémantique des Coordonnées**

Krioukov et ses collègues ont établi une correspondance sémantique précise pour ces coordonnées dans le contexte des réseaux complexes 5 :

* **Coordonnée Radiale (![][image12]) \- Popularité :** Le rayon représente le logarithme inverse du degré du nœud. Les nœuds situés près du centre du disque (![][image13]) sont les "hubs" connectés à une vaste portion du réseau. À l'inverse, les nœuds périphériques (![][image14]) sont des feuilles ou des nœuds de faible degré. La densité de nœuds augmente exponentiellement avec ![][image12], reflétant le fait que les hubs sont rares tandis que les nœuds périphériques sont légion.  
* **Coordonnée Angulaire (![][image15]) \- Similarité :** L'angle représente l'espace de similarité intrinsèque. Dans un réseau social, cela pourrait correspondre aux intérêts communs ou à la géographie ; dans l'Internet, à la proximité thématique des contenus. Deux nœuds proches angulairement sont plus susceptibles de se connecter.

Ce modèle, souvent désigné comme le modèle **PSO** (Popularity-Similarity Optimization), explique la formation des liens comme un compromis : un nouveau nœud se connectera à un nœud existant soit parce que ce dernier est très similaire (faible ![][image16]), soit parce qu'il est très populaire (faible ![][image12]).

### **2.3 Statistique de Fermi-Dirac et Émergence de la Topologie**

Une des contributions les plus élégantes de ce cadre théorique est la dérivation physique de la probabilité de connexion. En traitant le réseau comme un système canonique de fermions non-interagissants, la probabilité ![][image17] d'existence d'un lien entre deux nœuds séparés par une distance hyperbolique ![][image18] suit la distribution de Fermi-Dirac 1 :

![][image19]  
Ici, les paramètres physiques prennent une signification topologique directe :

* **Énergie (![][image18]) :** La distance hyperbolique agit comme une énergie de liaison ; plus les nœuds sont distants, plus l'énergie requise pour les connecter est grande, et donc moins la connexion est probable.  
* **Potentiel Chimique (![][image5]) :** Le rayon du disque détermine la taille du réseau et le degré moyen.  
* **Température (![][image20]) :** Ce paramètre contrôle le clustering du réseau.

Cette formulation permet d'identifier des transitions de phase thermodynamiques dans la structure des réseaux :

* **Phase Géométrique (![][image21]) :** La probabilité de connexion devient une fonction de Heaviside (![][image22] si ![][image23], sinon 0). Le réseau est strictement défini par la géométrie sous-jacente. C'est dans cette phase que le clustering est maximisé.2  
* **Phase Aléatoire (![][image24]) :** La géométrie "fond". La probabilité de connexion devient indépendante de la distance angulaire, et le réseau converge vers un graphe aléatoire classique, perdant ses propriétés de clustering et de hiérarchie métrique.

Les réseaux réels (Internet, réseaux métaboliques, réseaux sociaux) se situent généralement dans la "phase froide" (![][image25]), où la géométrie hyperbolique latente exerce une influence dominante sur la topologie.

## ---

**Chapitre 3 : La Correspondance AdS/CFT et l'Isomorphisme Réseau**

### **3.1 Principes Fondamentaux de la Dualité Holographique**

La correspondance AdS/CFT, proposée par Juan Maldacena en 1997, postule une équivalence physique complète entre deux théories apparemment distinctes :

1. Une théorie de la gravité quantique (telle que la théorie des cordes) définie dans un espace-temps Anti-de Sitter (AdS) de dimension ![][image26].  
2. Une théorie conforme des champs (CFT) définie sur le bord de cet espace, de dimension ![][image27], sans gravité intrinsèque.8

L'espace AdS est une solution des équations d'Einstein avec une constante cosmologique négative, ce qui lui confère une géométrie hyperbolique. Le "bord" de cet espace est situé à l'infini spatial. Le principe holographique stipule que toute l'information contenue dans le volume (le "bulk") est encodée sur la surface frontière.

### **3.2 Le Dictionnaire Bulk-Bord appliqué aux Réseaux**

Notre analyse révèle un isomorphisme frappant entre la structure des réseaux complexes hyperboliques et la dualité AdS/CFT. Ce tableau de correspondance, ou "dictionnaire", permet de traduire les concepts de la physique théorique en termes de science des réseaux :

| Concept AdS/CFT (Physique) | Concept Réseau Complexe (Krioukov/Serrano) | Interprétation TPDBT |
| :---- | :---- | :---- |
| **Espace Bulk (AdS)** | **Disque Hyperbolique Latent (![][image4])** | L'espace virtuel de routage et de hiérarchie. |
| **Bord Conforme (CFT)** | **Réseau Observable (![][image28])** | La topologie physique des nœuds et des liens. |
| **Direction Radiale (![][image29])** | **Échelle de Renormalisation / Popularité** | Le "zoom" du local vers le global (Hubs \= IR). |
| **Géodésique** | **Chemin de Routage Optimal** | Le flux de données traversant la hiérarchie. |
| **Entropie d'Intrication** | **Capacité de Coupe (Min-Cut)** | La bande passante maximale entre clusters. |
| **Trous Noirs** | **Congestion du Cœur** | Saturation des hubs limitant le flux. |
| **Renormalisation UV ![][image30] IR** | **Agrégation des Nœuds (Coarse-graining)** | Compression de l'information topologique. |

### **3.3 La Renormalisation Géométrique : Le Voyage dans le Bulk**

L'un des aspects les plus profonds de la dualité AdS/CFT est la relation UV/IR. Les phénomènes se déroulant près du bord de l'espace AdS correspondent aux processus à haute énergie (courtes distances, UV) dans la CFT, tandis que les phénomènes profonds dans le bulk correspondent aux processus à basse énergie (grandes distances, IR).

Serrano et Boguñá ont démontré que ce principe s'applique littéralement aux réseaux complexes via la "Renormalisation Géométrique".10 En "floutant" le réseau à petite échelle (en fusionnant des nœuds angulairement proches), on élimine les degrés de liberté locaux (UV). Ce processus de renormalisation engendre un flux dans l'espace des configurations qui est géométriquement équivalent à un mouvement radial vers le centre du disque hyperbolique.

Ainsi, le "bulk" de la géométrie latente n'est pas simplement un espace de plongement abstrait ; il représente physiquement l'histoire de la renormalisation du réseau. Les couches profondes du bulk (les hubs centraux) encodent les corrélations à longue portée et la structure globale du réseau, tout comme la géométrie profonde de l'AdS encode les états de basse énergie de la théorie quantique.12

### **3.4 Réseaux de Tenseurs : La Discrétisation de l'Espace**

Pour rendre cette correspondance opérationnelle, notamment dans le contexte TPDBT (Tensor), il est nécessaire de discrétiser l'espace continu. Les réseaux de tenseurs, et spécifiquement l'Ansatz de Renormalisation de l'Intrication Multi-échelle (MERA), fournissent cette discrétisation.13

MERA construit un état quantique en empilant des couches de tenseurs (isométries et désintricateurs). La structure de connectivité d'un réseau MERA reproduit la géométrie hyperbolique de l'espace AdS. Les tenseurs du bas représentent le bord (réseau physique), et chaque couche supérieure représente une étape de renormalisation vers le bulk. Nous détaillerons l'application de cette architecture au routage dans le Chapitre 6\.

## ---

**Chapitre 4 : Le Modèle TPDBT et le Routage Holographique**

### **4.1 Le Problème de la Navigabilité**

Dans le contexte des réseaux massifs (comme l'Internet ou le cerveau), le problème central est la **navigabilité** : comment acheminer un paquet d'information d'une source ![][image31] à une destination ![][image32] sans connaître la topologie globale du réseau? Les protocoles de routage classiques nécessitent des tables de routage immenses (![][image33] ou pire), ce qui n'est pas scalable.

La découverte majeure de Boguñá, Krioukov et Claffy est que les réseaux possédant une géométrie hyperbolique latente permettent un routage efficace avec une information locale minimale. C'est le **Routage Glouton Géométrique** (Greedy Geometric Routing).1

### **4.2 Le Mécanisme du Routage Glouton**

Le protocole est simple : chaque nœud connaît ses propres coordonnées hyperboliques virtuelles et celles de ses voisins directs. Lorsqu'il reçoit un paquet destiné à ![][image32] (dont les coordonnées sont inscrites dans le paquet), il le transmet au voisin qui minimise la distance hyperbolique vers ![][image32].

L'efficacité de ce routage repose sur la congruence entre la topologie du réseau et sa géométrie latente. Dans un réseau hyperbolique :

1. **Le Raccourci du Bulk :** Pour aller d'un nœud périphérique ![][image34] à un nœud périphérique distant ![][image35], le chemin le plus court en distance hyperbolique ne longe pas le bord. Il "plonge" vers le centre.  
2. **L'Ascension Hiérarchique :** En termes de réseau, cela signifie que le paquet est transmis à des nœuds de degré de plus en plus élevé (diminution de la coordonnée radiale ![][image12]). Le paquet "monte" dans la hiérarchie jusqu'à atteindre un hub global capable de "voir" la destination, puis "redescend" vers ![][image35].

Cette trajectoire est exactement celle d'une géodésique dans l'espace AdS. Le réseau utilise sa structure hiérarchique (le bulk) comme un raccourci dimensionnel. Les études montrent que ce routage atteint des taux de succès proches de 100% et des longueurs de chemin asymptotiquement optimales (![][image36]), validant l'hypothèse que l'architecture de l'Internet a évolué pour optimiser cette navigabilité hyperbolique.7

### **4.3 Vulnérabilités et l'Arbre Couvrant Minimum Hyperbolique (HMST)**

Bien que performant, ce routage holographique présente des vulnérabilités structurelles spécifiques, mises en évidence par l'analyse du **Hyperbolic Minimum Spanning Tree** (HMST).17 Le HMST constitue le "squelette" caché du routage glouton.

Les arêtes appartenant à ce HMST supportent une charge de trafic disproportionnée (haute centralité de charge). Si ces arêtes spécifiques sont attaquées ou échouent, le taux de succès du routage glouton s'effondre (jusqu'à 50% de perte), alors que le réseau reste robuste aux pannes aléatoires. Cela révèle une dualité critique : la géométrie qui permet l'efficacité (concentration du flux sur les géodésiques du bulk) crée simultanément des points de fragilité systémique (congestion des hubs centraux). Dans le langage AdS/CFT, cela pourrait être comparé à la formation de trous noirs lorsque la densité d'énergie (information) dans le bulk dépasse une certaine limite critique.

### **4.4 Les Vides et l'Échec du Routage**

Le routage glouton échoue lorsqu'un paquet atteint un "minimum local" ou un "vide" — un nœud qui est plus proche géométriquement de la destination que tous ses voisins, mais qui n'est pas connecté à la destination. Ces vides correspondent à des régions de l'espace hyperbolique où la densité de nœuds est inférieure à celle prédite par la métrique idéale. Pour contourner ces vides, des protocoles de repli comme le "Face Routing" doivent être utilisés, ce qui équivaut géométriquement à contourner une courbure ou un obstacle dans la variété.18

## ---

**Chapitre 5 : Flux d'Information, Intrication et Ryu-Takayanagi**

### **5.1 La Formule de Ryu-Takayanagi**

Le cœur de la connexion entre la géométrie et l'information dans AdS/CFT est la formule de Ryu-Takayanagi (RT). Elle relie l'entropie d'intrication ![][image37] d'une sous-région ![][image34] du bord (CFT) à l'aire de la surface minimale ![][image38] dans le bulk qui est homologue à ![][image34] 20 :

![][image39]  
Où ![][image40] est la constante de Newton (constante gravitationnelle).

### **5.2 Application à la Bande Passante (Contexte TPDBT)**

Dans le contexte des réseaux classiques, comment interpréter cette formule? Freedman et Headrick ont démontré que la formule RT est la limite continue du théorème **Max-Flow / Min-Cut** bien connu en théorie des graphes.22

* **Intrication ![][image41] Bande Passante :** L'entropie d'intrication quantique mesure la quantité de corrélation quantique entre deux parties d'un système. Dans un réseau de communication classique, l'analogue direct est la **capacité de canal** ou la bande passante disponible entre deux sous-réseaux.  
* **Surface Minimale ![][image41] Coupe Minimale (Min-Cut) :** La surface minimale ![][image38] dans le bulk représente le "goulot d'étranglement" géométrique. C'est la coupe qui sépare le sous-réseau ![][image34] du reste du réseau avec le coût minimal (nombre de liens minimal).  
* **Théorème :** La capacité maximale de flux d'information (Max-Flow) qui peut sortir de la région ![][image34] est strictement limitée par l'aire de cette surface minimale dans la géométrie hyperbolique latente.

Cette correspondance offre un outil puissant pour l'ingénierie des réseaux (le "B" de TPDBT). Pour maximiser la robustesse et la bande passante d'un réseau, il faut concevoir sa topologie de manière à maximiser l'aire des surfaces minimales dans le bulk hyperbolique. Un réseau avec un "bulk" trop étroit (trop peu de hubs ou de connexions transversales) aura une surface minimale petite, et donc une faible entropie/bande passante, le rendant vulnérable à la congestion.21

### **5.3 Les "Bit Threads" (Fils de Bits)**

Une reformulation moderne de la formule RT utilise le concept de **Bit Threads**.23 Au lieu de penser en termes de surfaces, on imagine des lignes de flux (des fils) incompressibles traversant le bulk depuis la région ![][image34].

* Chaque fil représente une unité d'intrication (ou un canal de communication unitaire).  
* Le nombre maximal de fils qu'on peut faire passer à travers la géométrie du bulk est égal à l'aire de la surface minimale (Min-Cut).

Dans le routage holographique, ces "Bit Threads" correspondent aux chemins de routage indépendants (disjoints) disponibles pour le multipath routing. La géométrie hyperbolique optimise naturellement cet empaquetage de chemins, permettant une utilisation maximale de la capacité du réseau.

## ---

**Chapitre 6 : Réseaux de Tenseurs et MERA (L'Architecture Discrète)**

### **6.1 MERA comme Réalisation du Modèle TPDBT**

L'Ansatz de Renormalisation de l'Intrication Multi-échelle (MERA) est l'outil mathématique qui rend la correspondance AdS/CFT calculable discrètement. Dans le modèle TPDBT, MERA représente la couche "Tenseur".13

Un réseau MERA est constitué de :

1. **Désintricateurs (Disentanglers) :** Des unitaires locaux qui suppriment les corrélations à courte portée entre les nœuds voisins.  
2. **Isométries :** Des opérateurs qui fusionnent plusieurs nœuds en un seul (renormalisation/coarse-graining).

Cette structure crée un graphe hiérarchique qui approxime le disque de Poincaré.

### **6.2 Le Routage dans un Réseau de Tenseurs**

Le routage d'information dans un réseau MERA suit la structure causale du réseau, définie par le **cône causal**. Pour calculer la corrélation entre deux points distants sur le bord, l'information doit remonter à travers les couches de renormalisation jusqu'à ce que leurs cônes causaux se croisent, puis redescendre.24

Cette trajectoire est, par construction, logarithmique en fonction de la distance de séparation (![][image42]), reproduisant exactement l'efficacité du routage glouton hyperbolique. MERA peut donc être vu comme l'algorithme optimal de compression et de routage pour un état critique.

De plus, les réseaux de tenseurs permettent d'aborder des problèmes d'optimisation (comme le VQE \- Variational Quantum Eigensolver) en utilisant la géométrie pour réduire la complexité de l'espace de recherche de exponentielle à polynomiale.25 Appliqué aux réseaux classiques, cela suggère que les architectures inspirées de MERA seraient optimales pour l'apprentissage profond géométrique (Geometric Deep Learning) et la compression de données sur graphes.27

## ---

**Chapitre 7 : Cosmologie Réticulaire et Dynamique de Croissance**

### **7.1 L'Univers comme Réseau Complexe**

Krioukov et ses collègues ont poussé l'analogie jusqu'à ses limites cosmologiques dans leur papier séminal "Network Cosmology".29 Ils démontrent que la structure causale de l'univers (l'ensemble des événements connectés par des cônes de lumière) forme un réseau complexe qui partage les mêmes propriétés que l'Internet : degrés en loi de puissance et fort clustering.

Cette équivalence n'est pas accidentelle. Elle découle de l'isomorphisme entre les équations de croissance des réseaux (attachement préférentiel) et la métrique d'un univers en expansion accélérée (espace de de Sitter).

### **7.2 Le Temps comme Coordonnée Radiale**

Dans cette correspondance cosmologique :

* La coordonnée temporelle cosmologique ![][image43] correspond à la coordonnée radiale ![][image12] du réseau.  
* Les nœuds "vieux" (apparus tôt dans l'histoire de l'univers/réseau) ont eu plus de temps pour acquérir des connexions causales. Ils deviennent donc les hubs centraux du disque hyperbolique.  
* Les nœuds "jeunes" sont périphériques.

L'accélération de l'expansion de l'univers (Énergie Noire) joue un rôle crucial. Sans cette accélération, la géométrie résultante ne serait pas hyperbolique mais plate ou sphérique, et le réseau perdrait sa navigabilité et son clustering.31 Cela implique une conclusion fascinante : **l'énergie noire est une condition nécessaire à la navigabilité de l'univers causal**, tout comme la courbure négative est nécessaire à la navigabilité de l'Internet.

## ---

**Chapitre 8 : Limites Thermodynamiques et Congestion**

### **8.1 Température et Transitions de Phase**

La "température" ![][image20] du réseau (introduite au Chapitre 2\) contrôle le niveau de bruit dans les connexions.

* Pour ![][image25] (Phase Froide), le réseau est navigable, géométrique et clustérisé.  
* Pour ![][image44] (Phase Chaude), le réseau devient aléatoire et perd son efficacité de routage.

### **8.2 La Congestion du Cœur (Trous Noirs)**

L'efficacité du routage hyperbolique repose sur l'utilisation intensive du "bulk" (les hubs). Cependant, dans les réseaux physiques, les nœuds ont une capacité finie. Si le trafic vers le centre dépasse la capacité des hubs, on assiste à un phénomène de congestion du cœur.32

Dans l'analogie gravitationnelle, une concentration excessive d'énergie/information dans une petite région du bulk conduit à la formation d'un trou noir. Un trou noir dans le bulk correspondrait, dans le réseau, à une zone de congestion totale où l'information est piégée ou perdue (latence infinie). Pour éviter cela, le réseau doit peut-être évoluer vers une géométrie modifiée (par exemple, en augmentant le nombre de liens transversaux en périphérie), ce qui correspondrait en gravité à des corrections de la métrique AdS.

## ---

**Conclusion et Perspectives**

L'analyse des correspondances entre le routage géométrique hyperbolique et la dualité AdS/CFT révèle une unité structurelle profonde entre la physique de l'information quantique et la science des réseaux complexes. Le cadre TPDBT permet d'unifier ces concepts :

1. **Topologiquement**, les réseaux complexes sont des discrétisations de variétés hyperboliques.  
2. **Physiquement**, leur croissance suit des lois thermodynamiques (Fermi-Dirac) et cosmologiques (de Sitter).  
3. **Informationnellement**, leur capacité est régie par des lois holographiques (Ryu-Takayanagi / Max-Flow).  
4. **Algorithmiquement**, ils peuvent être optimisés par des architectures tensorielles (MERA).

**Implications Pratiques :**

Ces découvertes ouvrent la voie à une nouvelle ingénierie des réseaux "Holographiques". Pour le futur Internet ou les réseaux 6G, l'encodage explicite de coordonnées hyperboliques et l'utilisation de protocoles de routage basés sur les "Bit Threads" pourraient permettre d'atteindre les limites théoriques de la navigabilité, de la robustesse et de l'efficacité spectrale. De même, en neuroscience, comprendre le cerveau comme un système naviguant dans une géométrie hyperbolique latente pourrait révolutionner notre compréhension de la connectivité neuronale et des pathologies de la communication cérébrale.

L'univers, l'Internet et le cerveau semblent partager le même code source géométrique : une architecture hyperbolique optimisée pour connecter le local au global à travers un bulk dimensionnel émergent.

---

**Note sur les citations :** Les références entre crochets (ex: \[1\]) renvoient aux identifiants des snippets de recherche fournis dans le contexte initial.

#### **Sources des citations**

1. \[1006.5169\] Hyperbolic Geometry of Complex Networks \- arXiv, consulté le janvier 16, 2026, [https://arxiv.org/abs/1006.5169](https://arxiv.org/abs/1006.5169)  
2. Hyperbolic geometry of complex networks, consulté le janvier 16, 2026, [https://named-data.net/wp-content/uploads/2010HyperbolicGeometry.pdf](https://named-data.net/wp-content/uploads/2010HyperbolicGeometry.pdf)  
3. Hyperbolic Geometry of Complex Networks, consulté le janvier 16, 2026, [https://www.mathematik.uni-muenchen.de/\~kpanagio/ModelsLitSS12/Hyperbolic.pdf](https://www.mathematik.uni-muenchen.de/~kpanagio/ModelsLitSS12/Hyperbolic.pdf)  
4. Hyperbolic geometry of complex networks \- University of California San Diego, consulté le janvier 16, 2026, [https://www.sysnet.ucsd.edu/sysnet/miscpapers/Hyperbolic.PRE.2010.pdf](https://www.sysnet.ucsd.edu/sysnet/miscpapers/Hyperbolic.PRE.2010.pdf)  
5. Understanding Networks: The power to predict pandemics, information spread, and quantum gravity \- Northeastern University College of Science, consulté le janvier 16, 2026, [https://cos.northeastern.edu/understanding-networks-the-power-to-predict-pandemics-information-spread-and-quantum-gravity/](https://cos.northeastern.edu/understanding-networks-the-power-to-predict-pandemics-information-spread-and-quantum-gravity/)  
6. An argument for hyperbolic geometry in neural circuits, consulté le janvier 16, 2026, [https://par.nsf.gov/servlets/purl/10120231](https://par.nsf.gov/servlets/purl/10120231)  
7. (PDF) Curvature and temperature of complex networks \- ResearchGate, consulté le janvier 16, 2026, [https://www.researchgate.net/publication/38081711\_Curvature\_and\_temperature\_of\_complex\_networks](https://www.researchgate.net/publication/38081711_Curvature_and_temperature_of_complex_networks)  
8. AdS/CFT Correspondence \- beuke.org, consulté le janvier 16, 2026, [https://beuke.org/ads-cft/](https://beuke.org/ads-cft/)  
9. AdS/CFT Correspondence and Quantum Error Correction \- Henry Yuen, consulté le janvier 16, 2026, [https://www.henryyuen.net/classes/spring2022/projects/adscft.pdf](https://www.henryyuen.net/classes/spring2022/projects/adscft.pdf)  
10. M. Ángeles Serrano University of Barcelona \- ResearchGate, consulté le janvier 16, 2026, [https://www.researchgate.net/profile/M-Serrano](https://www.researchgate.net/profile/M-Serrano)  
11. Network geometry \- Universitat de Barcelona, consulté le janvier 16, 2026, [http://complex.fmc.ub.edu/\~mbogunya/eotools\_files/files/networkgeometry.pdf](http://complex.fmc.ub.edu/~mbogunya/eotools_files/files/networkgeometry.pdf)  
12. Scaling up real networks by geometric branching growth \- PMC \- PubMed Central, consulté le janvier 16, 2026, [https://pmc.ncbi.nlm.nih.gov/articles/PMC8166096/](https://pmc.ncbi.nlm.nih.gov/articles/PMC8166096/)  
13. Class of Quantum Many-Body States That Can Be Efficiently Simulated \- ResearchGate, consulté le janvier 16, 2026, [https://www.researchgate.net/publication/23315808\_Class\_of\_Quantum\_Many-Body\_States\_That\_Can\_Be\_Efficiently\_Simulated](https://www.researchgate.net/publication/23315808_Class_of_Quantum_Many-Body_States_That_Can_Be_Efficiently_Simulated)  
14. Representation of a MERA decomposition of the tensor T associated with a many-body state, consulté le janvier 16, 2026, [https://www.researchgate.net/figure/Representation-of-a-MERA-decomposition-of-the-tensor-T-associated-with-a-many-body-state\_fig1\_23464316](https://www.researchgate.net/figure/Representation-of-a-MERA-decomposition-of-the-tensor-T-associated-with-a-many-body-state_fig1_23464316)  
15. Navigability of Complex Networks \- ResearchGate, consulté le janvier 16, 2026, [https://www.researchgate.net/publication/200775174\_Navigability\_of\_Complex\_Networks](https://www.researchgate.net/publication/200775174_Navigability_of_Complex_Networks)  
16. Visualization of the various routes of the Internet. \- ResearchGate, consulté le janvier 16, 2026, [https://www.researchgate.net/figure/sualization-of-the-various-routes-of-the-Internet\_fig1\_47438257](https://www.researchgate.net/figure/sualization-of-the-various-routes-of-the-Internet_fig1_47438257)  
17. Structural Vulnerability of Greedy Routing in Hyperbolic Embedded ..., consulté le janvier 16, 2026, [https://dl.ifip.org/db/conf/cnsm/cnsm2025/1571195911.pdf](https://dl.ifip.org/db/conf/cnsm/cnsm2025/1571195911.pdf)  
18. Geometric Ad-Hoc Routing: Of Theory and Practice\* \- courses, consulté le janvier 16, 2026, [https://courses.csail.mit.edu/6.885/spring06/papers/KuhnWZZ.pdf](https://courses.csail.mit.edu/6.885/spring06/papers/KuhnWZZ.pdf)  
19. Void Traversal for Efficient Non-Planar Geometric Routing \- Kent State University, consulté le janvier 16, 2026, [http://antares.cs.kent.edu/\~mikhail/Research/voids.pdf](http://antares.cs.kent.edu/~mikhail/Research/voids.pdf)  
20. Bit Threads and Holographic Entanglement \- Brandeis University, consulté le janvier 16, 2026, [https://scholarworks.brandeis.edu/esploro/outputs/journalArticle/Bit-Threads-and-Holographic-Entanglement/9924086388201921](https://scholarworks.brandeis.edu/esploro/outputs/journalArticle/Bit-Threads-and-Holographic-Entanglement/9924086388201921)  
21. The thread embodiment of holographic quantum entanglement \- arXiv, consulté le janvier 16, 2026, [https://arxiv.org/html/2501.10691v4](https://arxiv.org/html/2501.10691v4)  
22. Quantum Max-flow/Min-cut \- Purdue Math, consulté le janvier 16, 2026, [https://www.math.purdue.edu/\~cui177/Papers/8.pdf](https://www.math.purdue.edu/~cui177/Papers/8.pdf)  
23. Bit Thread Formalism in Holography \- Emergent Mind, consulté le janvier 16, 2026, [https://www.emergentmind.com/topics/bit-thread-formalism](https://www.emergentmind.com/topics/bit-thread-formalism)  
24. \[PDF\] Convergence and Quantum Advantage of Trotterized MERA for Strongly-Correlated Systems | Semantic Scholar, consulté le janvier 16, 2026, [https://www.semanticscholar.org/paper/12823da9009c7fe6c29daaf1eb5b85ed78f95199](https://www.semanticscholar.org/paper/12823da9009c7fe6c29daaf1eb5b85ed78f95199)  
25. Isometric tensor network optimization for extensive Hamiltonians is free of barren plateaus, consulté le janvier 16, 2026, [https://arxiv.org/html/2304.14320v2](https://arxiv.org/html/2304.14320v2)  
26. Convergence and quantum advantage of Trotterized MERA for strongly-correlated systems, consulté le janvier 16, 2026, [https://arxiv.org/html/2303.08910v2](https://arxiv.org/html/2303.08910v2)  
27. Brain-Inspired AI with Hyperbolic Geometry \- arXiv, consulté le janvier 16, 2026, [https://arxiv.org/html/2409.12990v3](https://arxiv.org/html/2409.12990v3)  
28. Comparison of hyperbolic embedding methods for real-world networks: Machine Learning versus Network Science, consulté le janvier 16, 2026, [https://mscest.cut.ac.cy/publication/2025\_zhou\_haojie/2025\_ZHOU\_HAOJIE.pdf](https://mscest.cut.ac.cy/publication/2025_zhou_haojie/2025_ZHOU_HAOJIE.pdf)  
29. arXiv:1203.2109v2 \[gr-qc\] 26 Nov 2012 \- CAIDA.org, consulté le janvier 16, 2026, [https://www.caida.org/catalog/papers/2012\_network\_cosmology/network\_cosmology.pdf](https://www.caida.org/catalog/papers/2012_network_cosmology/network_cosmology.pdf)  
30. (PDF) Network Cosmology \- ResearchGate, consulté le janvier 16, 2026, [https://www.researchgate.net/publication/233539876\_Network\_Cosmology](https://www.researchgate.net/publication/233539876_Network_Cosmology)  
31. Navigability of Random Geometric Graphs in the Universe and Other Spacetimes \- PMC, consulté le janvier 16, 2026, [https://pmc.ncbi.nlm.nih.gov/articles/PMC5562713/](https://pmc.ncbi.nlm.nih.gov/articles/PMC5562713/)  
32. arXiv:0907.1478v1 \[cond-mat.stat-mech\] 9 Jul 2009, consulté le janvier 16, 2026, [https://arxiv.org/pdf/0907.1478](https://arxiv.org/pdf/0907.1478)

[image1]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAGEAAAAZCAYAAAAhd0APAAAD9UlEQVR4Xu2ZWaiNURTHlwwRMpOhLh7IUJLhpnhBImOiTG8ylSdCJBnyIHkgQ0l5MhTKi+FBXMODUqRMKblEQiihDOH/b33rnn32+YZ9z73OueX71T/O3t/Z37fXWnut9Z0rkpOT82/oFKkxtIJa+4M55TEWug7V+BMZ0AknoC7+xP/IMOgwdBR6Gel89Jk6AE2D2toXHOiAp1CtNz4Eugt9hK5AHYunG9gFXZKW4Yidonv/Bc3w5hoDg2sN9A36IwW7TYXm20U+PaF50CboN7QNWhBpOXRNdLE79gUHGpiG5I1dukNzRb9HJybRA7oNbZTSNSoNA2kF9EE0MMtlmeielkIroelQB2gP1Nu5Lpbd0AWovT8h6iAatK8z1gc6KMnGo3NDNsR1HouuVW1WSXrQcE8WoL4YyK59DNp1HzTIn/BhumBU09g+baCzok6gwYw5okcsiXFQnYQVbG78lT9YYaxGcV/NyXFovyQHawODoTfQRH8C9IfqRZ1gC/FfLj4g+hwHo4pR4ML0E/cwzJVcv5owyh+K2sLgs8ZlhsbAejvBH4yD3vcjnfAhmK85xwJsdBOtEUkF106PFTjmRK7DtHMomncZA331xioNA/CnFPY0HLoBPYdG20VlwJpJB6fCdFEnamjrjih2NregmVLaz2cZzTbUDzothUjgPU5JqRMsCrNSFzsNFjg2EO+gL9CGaDyO0PcXCxquu1A0PTJwuM/vEhjJCdAJmbBwsoDyAULJcoIV8stSXJinSPzpsUDIMthq0XcSS4M8qTxd50Q7Mp+REp/+fCzlsq3cKgWnMvjYboeskQS7o0zYStFg9d54GowMRkgczKHssrjma9GiNLToilJCncDCOdAbo1NZnx5JscMZyUecz2mwwWAQ8pmvQktEv98cBK1zTPTmPI6hpJ0ERik7nXpoEvRM9Nq4om90hm5KthN2+AMRjFzWHEbyItH3m3uiL5shbBG1AU/w3uj/JyU5zTUrVmB5U3YzoaQ5waLKnGonjb1yL2ixlNYE9tcvJD5VudDAabCY/oDeitaKkCi0k8saxkAxm7wXTUVsLrLedZoEH9TSRlbKcLH3Cj6wi78hsk70HrOhM9CIaNzFCnk1cIOGwcEOkae3TvRk8mQ0pSYkMgr6LGocVxwPZbuURoht4L7oOwGpgR5AT6C1Er8hpoFP/mCFsCBhCiN8vvWiJ+qipL8LVR0W57gU1lVKX3DYZST9bmKnh51UNWDeZ2flBwdPgf/e1OJgvqXhQvJuGmwj2SJn5fucBNiR1En5P0XXiqav8f5ETjg8yvZ3h3LaOf7NIfE39pxwaPzN0Cx/IoN20GR/MCcnJyenovwFdLnBFLP70nMAAAAASUVORK5CYII=>

[image2]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAaCAYAAABRqrc5AAABBUlEQVR4XmNgoAxwoAuQAkSA+DAQT0KXIBWIA3EQuiCpoAiIedEFiQErgHghEO8E4ltockQBeSAOhrJ1gPg9khxRgBGIpwAxD5RvA8QPEdLEAWkgfoDEB4XHaSQ+HAig8WG2ggDIkKtQthkDxCvRQGwJV8EAiarnQLwaiPWB+BAQPwPiYgaIV0A4B4hLGCDeWgrEC4CYkwEK+IF4DRCXA/F/IH4NxFZA/BGIDzCgugjmWpChgkjiDC5APIsBkvpAhmRAxUHs5UDMAuXjBZ5AbMcAScYgLylBxe2BmBumiFgAsrkVXZBUADIE5CqyASjwkL1CFgBp3spAYfngwACJ4lEwCmgGAJFtJjrqsj/IAAAAAElFTkSuQmCC>

[image3]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABcAAAAaCAYAAABctMd+AAABSElEQVR4Xu2UvytGURjHH6GI/Mi7KKWkZFBKKWJRBimbSfkXEJvBbJPJYJGJZJPCZBMjGaQw2Bj8A3yenvP2nvt03x+473Y/9Rnu9znvOfc857xX5Pe0BOvCMk75MCtW8As/cdrV/kwDrvowK2Zxz4dwiI+4hqd4nixXpxVPcMIXYATP8AqH8DlZrs4YXmK3y/XW9OMTLoi1bjwxogaW8MCHAb05rzjsC+Xowp7oeU7sdkxGWRFt164PPR24jR94g7c4GmqdYgf1jYvYFnLlXqwlFXnDa+wLz9q//VJZGnFebIELbA+5LqRjy6KH8o6DUaY/SNuu7uYOe30hDZ1kR0oT6Rvq22+JLRqjvd8UG9/kaqnoKWufB3whC4qT+zucCQV8kPTJN6TG7VdiXZJfOD2HGbHb8W+axT6jR2L/xBc8jgfk5OSk8wMtGSzt966c3gAAAABJRU5ErkJggg==>

[image4]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABYAAAAWCAYAAADEtGw7AAABMElEQVR4Xu2TsUqDQRCEJ4UhMQQR8g5iYWUQxNbGRkQsRB9AnyAPYmmhlViphdiJTcpUPoK1SCoLG5OZ7P162WwSjZXiwEf+2/n/Y2+yB/wSLZFTcuCNWVUht+Qyrfcz70fSxjfkMa1XM2+gPXIBO07OVvJ9XWwkb46U0/N2+v3QCj4375FjskMayc+9J+cVqsJiCXUC+7jk6loXG+udSC1y74vSMnkhr96AZae6fL3n1YR1HGoX1lHHG9QRzGuTuvPWyAMsrkPnDVTEcO4NWC2KoQY7vryCIakLdSOji9EJeE6eTvUt5TEsOk8aF8NU5TFEExHFMFXqUJ3q4yh8zetMMeRjNnIlYbVxYzZRV7COrsm88xZgt+kMdnW/pHXyhuFREXdkk7wHXvQf/OuvqA9Y81AiXq55ewAAAABJRU5ErkJggg==>

[image5]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA8AAAAaCAYAAABozQZiAAABFUlEQVR4XmNgGAWeQLwQiG8A8SMonoWEG4FYDa4aDWgCcQgQLwXi/0D8EMoH4WQg3g8V54dpwAYmMUAUzUETZwXi+UA8HYhZ0OTAgAeIDzBANEejSoFBORDfBWJxdAkQ8GOAaDwNxIJocopA/ASIi9HE4aCVAbeTQYEGkgOxMQCyk/OAWBKIA6DsO0B8HYi9YYrRgRIQPwfinwyQEAfZtIUBYthuIBZGKMUEuPwbAxVfxYDDySBwgAF7KLsA8T8GSLyDvIIVgJz8CYj10cRhgYgzikAAm5M5gHgrVO4AAyRQQSlRGkkNWBFIwWooG1kcXfNKIDYGSYKcCHIqSBIZL2dAJEEbIP4KxblAXArEjFC5UTDMAQBbwESmc4JngAAAAABJRU5ErkJggg==>

[image6]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAsAAAAaCAYAAABhJqYYAAAAwklEQVR4XmNgGAUDAQSAmAeJzwrEzEh8OFAD4idA/B6IO4HYHIivAfEFIJZHUgfmbIWybYD4JxA/AmJVIP4PxEVQOTCoA+IYKNsUiL8B8Xwg5gPif0DsAZVj4ADiVCAWhvLTGSCmRUP5+kDMCGWjAEEgPg3FIDZWAAoBkMnGQPyVAeIEmGkRUDkwUGSAhMJbBoQTkD20Boj5YRyYaduA+BADqntBivygbLjATiDeAsS5QFzKALFlKRBfZcDhuVFAOwAA6pEhOYcb9LQAAAAASUVORK5CYII=>

[image7]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACsAAAAZCAYAAACo79dmAAACYklEQVR4Xu2WO2gVQRSGf1Eh4iPxAUEURLtgwMIHCJpYWGihha0IdlrYhZg+IZXaiJXa2KqdCEJErkkjWFmIlZCIaCWCoKDi4/85O/fOPZPZ3cT1VveDn3v3zMzu2XPOnB2gT29Z7w09YoDa5I1l7KaeeON/QI4NO9se6rmzZRmk5qjLfqBBlLVJ6j31iDrUPYwjhUpZQ83AbrDBjTXJdeoNLIriBSxIAfnx1NkSbiFd2DT7qfvo3hN/qPPRtaj0RW87640NoojJibPOLmennO0U9YM66extflGnvbFAO3Qoutb/Fe1aMkp9pnY5u5y95Gz7qI8oCd4X6oA3knPUK9hijc/DUvQBFq26XIE5Fq/ZXNh8kGRfoB7DukYXG2GDmhSjNNyGPeAmOl3iBuwh64rrKtQOtft/w+4X1KJeUlvbMzvco5aonX5AKW0VvzF64zF03lTpEVuo8TCpBoepb9RrZ1cAcqmWs5+oET+QczagBVqYpKQmZ2CZeBjZFE1F9Whki5GzX6mDfqDKWe1gPWy1BGfjKB6jfiLf0+WsSkcl1IVq7y3Sz19A6WrC2dCiQhv73p6Rkq1ZoZpSbXlCG9HOzBEys4i0NQlFT+cNObiNegbbYLkD0w5Yfd/1AwHVh+934gSsB/vGHaNITcDqOqmxAp0BlFZl8Bry6Re6h/zxX7Y2LdgG8O1oLbW9+K3iDpbv1YG6R0AFTS+21w8E1EPfoWRCDR7AUvivhJIp/egch6VJB46VomNdsnNXgQ4vKqlK9CYXUb6ZcjQRUT3/KvIbL0ELLnhjj9DXctob+/SJ+AtQkmnWB3VgVgAAAABJRU5ErkJggg==>

[image8]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADQAAAAZCAYAAAB+Sg0DAAAC2UlEQVR4Xu2Xz6tNURTHl1Dkdx7yozySKPUGopQhRWFiQJmYMTAQA2VkYkzqpURMpPwYGChhcEvhDyClFBIjRMiPwvpYZ7v7rrPPPfvcewdP3U99u521z9l7r73XWntfkSH/J5MLNeG16rA3DoDpqhuqmcXzVNWcdnM9fDCumuQbavitOuGNDWC8+YXisdeq3knbCX4vS+b8cOas6oJvqIHOv6s2+YYGPFLdVz1WXYvsu8QWKwanj0qGU7tVz1WrfEMNI6rbYuHRC1tU+8UmuEIsfANnVB+i58Ar1UZvjDkk9uE635DBAdUib8yAvLgjnRPG1lItFgu3N6ptUXsA24/iN0lLdUs1zdnrYFUvemMme8XC6UpkY7efqMbEwu2BpItAeI9vp7i2v3xRHffGAioe+ZV6nie2GE1hkuQNDjHxQCgCy1QnpbrQsJAUhxeqpZ1NBh1v90axgW+qPqt2qPaIdUKcbxZzbkl4uQF8+1PKE2IOzIUdIPlnR22eY2J90FeJt6qVzkanxDj2T2IFY1RsIAY9+O/N5twT6+Oh6lyhS2L55KtaFRSTX2KOlXgplogxo2LFgrxiECpOIOxOrzAek2FSgRBuhH8O68XeLTnExFIOxfhY7xd2nLAlVwJUS8bhCMih0iHo5hCJnwrJfmAiHKSzimfOMBxh1ypLsWOD6qtUOMSKUSpTsBItad+nBgGhdV3aJZdbBreNq9JZUbuxU2xHj/gGoGGfNxacl85Yz4Fv6BNx3nhOq56KHciU4PdSc/InoKyzMOReCeI5TvpAOLmTtb4LW1UfpboKLVDdFatyhN7qzuZawrwqr1ycuJy8lGrPXG9oALuecggoRgvFjoGmhIpIFU7Cin6T/ITMgVA6Jc3DNQccIaq4zFayXOz6zm2gX7hhcDccZKkPsFAczKk7XgkS85k39sAM1RrJ+M/SA/zNYfGzIT7D+TDR4Cykgg4ZMhH4Ay9OhG54gQorAAAAAElFTkSuQmCC>

[image9]: <data:image/png;base64,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>

[image10]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAZCAYAAABQDyyRAAABUUlEQVR4Xu2VvUoEMRSFj6igYKdgoeAPgoiVCIJgYWFjYe8bbG/jE/gCYm9hYeMDWAiKWgjaipVgYSeWFir+nMPdIbvX2d1khFTzwVdMbuaQ3E12gJr8bNBXP5iTffrjB3MxQi/osxvPxgKs/Qe+kAu1/5QO+0IO1P5zuu0LBaO0r8tzDENof6/1eZbe0JlmrY0V+khv6TysVVf0EhYQgzLuEHKU8YCQM0gnUbIp3ctjugO7HoewyV/0hS6GqV1RxgBCjjLWEXI6stn0hH7DFiTW6FwxKQJlaAFFjuhHQs49faITbjyFMYScZD5hq9cuqqLdFjnJ6Hfb9YOJ6P1KOeOw1qmFnTiDhb/TVVcTytAN6JVTyjLs9P+5Ii006AfsgG25mlDGG3rnlKLTqmsTwx7KF6AM7Tw2pxL6Dz+CfVSyM0Wv6ZIv5ELtnfaDNTX/5RdEPzsrLayBNQAAAABJRU5ErkJggg==>

[image11]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAmwAAAA6CAYAAAAN3QXmAAAGF0lEQVR4Xu3da6isVR0H4BUZFFmRhRkqVgRRhiKJUCSEFBRRkRUVBfXFUlM/JBVE4PnShxCiQoIiiD5EFN2gCxGBuwsVGV1AK8jgKGKQiBgkRJitn2vezprVnr1npnn3PnCeB/4473rfvWf2IJwf61oKAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAADAme2GWo+NjSvcWOtkrbcP7QAAzOjO0gLbs8Ybg/NqfaPWObUeGO4BADCTc2u9r9avFrXKh2s92l3v1XpOdw0AwAzSo/az7nV62Z5x6vZ/PaG0eye6tntqvbi7BgBgBu+udXt3nVD2ju568vxa/6z18q7tkVrP7a4BAJjBz8tyj9q1tf5d6+quLb5QWpi7v9a9i//mOj1vAADMJEFt7E3LnLQEsR90bU+r9dNaHyqtRy310sVzAADM5OyyPBTa+2NpYewpi+uX1fpHWV5g8JFaX+muAQDYsdeWU4sNRtOebK9ZXE+BLSEv0jP3y7I8nw0AgB37Q61Ly6khzrFuK22RwZW1nlnrjlpnPf6TpfywtF44AABmkqHO9KCtU19b/MyJ0oZEn1jrb7UuX7QDABy7hJYTY+MRel1pG9Zmwv+Th3vreEuti8bGLWWD3cNOQvj8ogAAjsSzS1stOU2+37U/l7YPWoYmf1za8VD7hatXlnaqwDSHbF3pHZt6yI5S/qaLx0YAgDlksv247cWupLfqrd31dMrAfisv8zn2yuaB7e+lLS44ahk6/VSxRxsAcIA3jA1bSNj44th4iLzvl8bGFV5dWkDL9hiTad7YaJvAdn6tz4yNRyib775xbAQATi9PrfXZWjePNxYSPl41Nu7ILgJbVkbujY2H2CSwPanWJ2ud17UlrP2ru570gS1nd6Zn7tO1nlfrbaV9zy9ZPDtJIHzX0HaUHizHGxgB4Izy+lq/rvXmWn8pbUuHW0pbKbiqB2Wv1jXd9TdrPVTaCsNJwsr7u+teJtl/otajtT5W6wOlTbrP7vrr2CSwXVHrPaUFre/XelOtk/0DG9gksI0uLC2wZf7XaOxhy/Yaefau6YHS9klLSJ7kKKn83HHZK8ufDwCY0Y/KqYnwCSPZnyuT8cfhvN5Hy/L8pbzOJqz3lLbZagJSfm9/hmUvE/2nI5IS9DKB/YHSVkyuY93AluCTvyn7juW9EhS/s3i9jW0DW76fzPk6UVrP22gMbDF+//lu+4PYp7/ruHy9tM8EAMwsQeKcxesEqPSwZW7U3BIQs4VFhgezQvIgryhtiLCv9M6NbekpHKVH6rLSevo+Ptw7TL6b8T3yvj8Z2vK+fc/Xfh6u9d6xsbMqsPXBtA9s+Wxf7q576R3dde3Xk5fAKLABwBFLcEqAmna7P0gCQ/b/eqy0HrKnL99+XAJghjtXuaC0IbX05h3k/wlsk4SbzPnaxK4CW4Zkr168zu/sh5Inmwa20MMGAGeQKXB8ryxPiL++LB8G3ss8t4u666tq3V3rkq7t9nLwWZQZVl01x+0w6w6JTh4p221KO9p0SPQXpQXb6TiohMbfLT3RbBPYPlgO752cU8J2/p8BAGY2zSNLMPhrrfu6e+lBWbWh7DvHhtJCX37Xt0sLb5kvlh6l/SQ85R/7bQPHpoEtn2sXNglsmb+X9x1rr3smsl9bfu9va72otNCW3sc8e11p31WeySKQ9NZlP7c4HVaJbjrMDABsIRPgExS+W9pu/HfW+mqt3/QPzSA9Sln1uCrQHWaTwJYAdHJs3NImgW1uGbq+o7TtSY5DDodf1QMLAHAsu/tH3vdzY+MxyorXTY+myhBt/o4MryZ0pSdv1WreVbI1yQvHRgAA/ldWwGYoexN/6l4ndN1f2nYj68rw7O/HRgAAVsuw8rfK+sdajYsZstdbziTNkPg6bi377yUHAMCOZGuSfhuSBLb00r2gawMA4DQxLf64crwBAMDpIYsWcp7rtqt1AQCYSQLazWXz0x8AADgi2dqj3yT5ploXdtcAAByjy0ubszYdl5XKUWPrrjIFAGBm41FZqawUBQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA4c/wHoogO3I3Ee/8AAAAASUVORK5CYII=>

[image12]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAkAAAAaCAYAAABl03YlAAAAiUlEQVR4XmNgGAWkAgECfIYgIH4OxKuBWB+IDwHxCSAuBmJGkAJ+IF4DxOVA/B+IXwOxFRBbA/EBIOYBKXIB4llAPAmqKAMkCAS9QLwciFlAHE8gtgPiwwwQK5WgiviAmBvKhgOQKa3ogugApAhkKk4AchyyVVgBSHIrEHOgSyADBwZIEIwCCgAAxm8UgTb9h3UAAAAASUVORK5CYII=>

[image13]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADEAAAAZCAYAAACYY8ZHAAABi0lEQVR4Xu2WzStEURjGH6GIsqDkY0GJBTullCULCyxslD0bNjbK3sLWWiwltiJZTJSNtR2FJfkDJB/PM++d6d7Dvded7sjU+dWv5pz3zNzzno/3DuDxeGqZkcAmN1ALtNBtehD4QrciI/454/SVbjr9SkqxP2eOrrudKWiyn3TR6V/G98TQTusS2nkwCjsOzW4ghlZagCUxEw0V2+ewo1ZkjN7RazoEy/6SXsCSyQtN/pBOuYEYuugD4pO4oR1qTNJ9ugYbvEcb6Tt9psP2ndzQ7q7QEzfwA2lJKKYxmA48oh+wpMQEHQg+x6Ht1o9ktZtu0AXYgsXx6yRKaGvuaU+4M4VV+lihT7BJuBc2TOYk3mC70RDurBK9sDuXtAsi7WIXYGPKaGDW8lcJbfSYzruBGHZgc1NJDaM7rAJUphOhm15F9JxT2u8GEtBKn8GqZ4m+oB0p1arfqkp5vxdcZukusj9Hx++KLgXewt4REeqRfj7zQH/cImc4A5qjioAq2iCyL4TH4/F4svMFF0VTbR8SMnkAAAAASUVORK5CYII=>

[image14]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADYAAAAZCAYAAAB6v90+AAABwklEQVR4Xu2WvytGURjHH6EIEUqSRRaTjZQwGBhIGEwMFBkpjEomZVAWBpkkBiUTg7BZGRUGBvkDJPH9Oqf7np73173v65a3zqc+ve99zun2nHue89wr4vF4PAmm4QN8tr+HcMe6CJsTUwuLTngFv+EtnIDjcB7e2XhpMLvAeISfsFvFyT68gBV6IG42YJkORoSLYhk2qHgVvIbHsMQdqHEvQKW6/gtOYZsORoTllpQ86IIfcNgNjsJXeATbxdTxi5gDWeTMy5dla65wMVzYgopXiylBjgX59ovpKlt2YM7G+f9Akp9MvnTAG9iqB0LAc/UG9yTRDZnnLix35v0yCHvE1Cd3rcXGeyX7IWS5NubgmJiWnZRMFrjbugzXxCyOvymr6x2eSbTDvSImwaiyzJnMlISHi+GidBkOibnXpaTpCxxc18EYYBWwLW/qgSw0iWn1us3PSoiFsSzjhE99Gy5JmrLJABfEVq/bPHeRuad8f/FcRS3DXOBODehgCOrguaT+sri3cd6bnIjzadUn+bXhsPA9Vq+DGWAFMWntqjNnEn7BJzgjpjEFFFvjplail2AYuEMjYr4b47i/x+PxeP4nP1KLYv0l6v/AAAAAAElFTkSuQmCC>

[image15]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAoAAAAZCAYAAAAIcL+IAAAA3ElEQVR4XmNgGHSAFYjFgZgDXQIGGIE4HIifAPFmKI0V5ADxcyA2g/KjgVgRIQ0BYkB8CoiFkcSMgbgViQ8GINPK0cR8gXghsgDI4dcZICYggyIgnoQs4AHE/4CYB0kM5LGlDBDFYMALxIeB+D8Qz0LCIF+DNCvBFMowQILhLUwACtIZIJpZYAIgd30F4tMwAQaI5BoGiEI4gCkEScAAyDpQeF5BEoMrRA4GUFCBTItBEgP7bgoQ7wBiTiCeA8R7gJgfWREMyAPxRSheBcRCqNKoAJRiBNAFRwFRAABeBiYByZSPBgAAAABJRU5ErkJggg==>

[image16]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABoAAAAZCAYAAAAv3j5gAAABi0lEQVR4Xu2UsStFYRjGH8WgFCIWFpvYZLMqRQYW5f4BBptBmZTskolBRouySCaxiMkgg5QkksFESeF5es93z/d95xw5w110f/Wre5/vu+97z/nec4A6NWKcdsbhH2ijHbQhXijim26gxA/IHr2kp/QgWsulG9bolQ5Ga0X00E3aRNvpRbicRU3O6Qqs2QsdCHZkmaNfUbZD+6IsQD/ahRVXEzVT0yL0x67pnZe10GM65GUBXbBLHoWdzRqs0aO/KWIetmfby9T8lvZ7WUCF7tPm5LvOR+ekQnlo3yFsfdLLh+k7rGGGGdikuCYO12w5ysUU0nPUFWkYtuh9kmdopSd0LF6A3UKN+Q3tjdaWYAXXvUzP3hX99LIqRVfj0KGq4GKUa7KUz3rZCKzJmZdVOYLdhiIaYQU1Xf59VyMVVXHHKmyvpjeDGmkkf+MDVkBT5lCjN6Rj7EZdz6FeQwE6FxUoo/u3GpRnpGf7RKeTzwH+eJZR7zOhQVmgD7D33ESS1Qy9sXOfmTp1/jk/jfxk38kfW0MAAAAASUVORK5CYII=>

[image17]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAZCAYAAAB3oa15AAAC5klEQVR4Xu2WS6hOURTH/0KR9yOPKO+BKAOPIhOvIjGhKGViwMCILsWEgYEykpsJIUlKSYiBdKNkZkKKFPIYSEqRRx7/v7W3vc+65/u699xzv666v/p3vr32Od/ea++19tpAP/8vA6lx4dmbDKZGeWMdtFNt1ADfUTOa/AXUPI5W5XR4tgLt9F7U6MQmarY39jKvqCXeWIXd1EdvbAFrqe/hWZnhVAd1w9lbwXjqMXWRGuT6/jIBxRNlIjUka4uF1GfqgLPn6Bv9V6N2VRT/SuYX1JRiF7CIekk9oubAEuYu9YU6iJSs26jf1LrQzhkLG+AN9ZZaT20Pv6Vp6dXK7Kd+UMtz41LqMtLkziBNOK747dA+R72jZoZ2zmGkU0JP/ddGajJscbaGvp6wmvoFc+Qfy2ADaeJx0Ig8lcdPQ1sOaDKaVI5Cb1bWHoPkqJxZEJ45+1BeoFbBFrOMuKAFByJKEL+6O2FOdcAmeQnlDng0kBLd51DOE2qqs42k7lMnnT3S1IEYKsNCW5mu0JIDx4Ot0Q545HizRK/KYlheljqgiR7J2jOo19Q3WJ4IOfAJFhIenVrKnei44jUiu6ppT9kAm+ce36EzVh0nkGJVxeo80o4InT56z8eotvY9zLFd1E+k8JhEXQu/FfPHYDuYT0JjqrLPpZ7B/q8MLfAH2HsFlKwPYLF+j7oKO0r9XSfuSgypyFDqIXU9SI7oSFbOKLdWhvemUytgOzo/2MTo8NQB8hwl5zxSEb0FG6+AYkrSSmirFQ5lKDxUCTUpj76T4g6qePniGDmEkknAVrhR8mvVtfq6yhTQy/ooj9lmrKG+emM3iFcCrXK+0gpVHSKNkl8T1+4rCgrcRCpgXS02qqpbvLGLzIOFqxIyp1n4aFflXFndwOZMnZKjCSpuVa+3ZSGi8NHpVXZR0/W9jqtIATnbTo3wHd1AK6u71lnYruwo9BoqrKe8sa+gnbhC3aGOovOp10+f5w/imoM4RZcH5gAAAABJRU5ErkJggg==>

[image18]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABcAAAAaCAYAAABctMd+AAABYElEQVR4Xu3UPyhFYRjH8UcoSv53JYNISkqKSboTA6VslFImk4VBWY1SymJQJolsV7IqWZTJn4VCVkwm+fN97vsc53Wi3HPuxP3Vp3vOc473PO9zzyVSSCH/LxWoQ5GdV1stcfZxj0cco9POnzAn4QNzjnbbZ8cNuMQrunCFa6vHyrx3XI9z3GAW7zhAuXfPr1OMKe+8B8/YFbdgGpXedY3uaAalP9S/jc51Ay/oj1yLHX0jdAfBSPwZd2DQjnNOCmcYENetdq0jKRG3k1WMf94tksGFuIdqdDQL2MYp2q2eTTDjVqzhTcLFx7An4bvegmZxOxuy2qS4poJdj1g9G/1DXeAQSxjFg9W2UBveKt3idqGLBGMbFteINnlnn7FzK67TNvn64HVsSoIfm+YETVhEldVqrD4d3BQ3R1hBr1fLy0g0+h2VRWoT4jrXHeQtumgjdrAcuZY4+o7rv+U/lg9YxDk1/qCLVgAAAABJRU5ErkJggg==>

[image19]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAmwAAABACAYAAACnZCtBAAAFKUlEQVR4Xu3dT6hmYxwH8Ef+RBjjTzRREzFS/k1YEDWhZGHK+JOYhUxhQYpCNhhZMNkYpImm2VjIgsZkyGIaC0VZsVFTRixmIaVsSPx+nnO655555877vnMv573386lvnfOc973de1e/nuc8v6cUAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACA2bEqsqM/CADA/29LZHNkW2RX7xkAAAPyTFGwAQAMmoINAGDgFGwAAAOnYAMAGDgFGwDAwCnYAAAGTsEGADBQp0UuiLwV2d1cr573CQCARXJ8ZHvkhP6DY7A+src/CADA5I6LPB05o/9gEdwVWdsfBABgMl9FXuoPLqKfIo/2BwEAGN8vkcv7g4vojci3/UEAAMZzTeSR/uAiOz/yQ6lLrwAA9Dwceb25XhXZEbl/7vG/xdqNnfuuF0v9bhZaTzTX0zg5sidyTv8BAMBKl8ucuZEge4R9H7m4Gd9U5mbVPo+saa5bN0U+bK6zbcXfkUsjhyJ3tB8KV0ZO7Nzn9eOd+678HW7tD3YciPw4Rra2XwAAWA6uiJwZ+TpyWWf8ycgHpbbw2FdqUdZ1Q+SU5vqqUj9zrLLQ6xZ7S2HDCg4AMMOy4PqtzBVluby5M/JOc/9F59koD0Re7g9O4b8o2AAAZlIWZrmk2cr31f6MnNvcj1oSzZm5W0p95+y7yEXN+NmRUyMXltpbLZcxWy+Uusy6rzPWZUkUAOAIcjn09859FnB/9e7bgqz1a6nfaYu705vxzaXO0F0dua/UYq6VS645c5cZJTcsdJdll4P8P+QmjjyWakuxCxYAmFLOrn0S+bjU5c+by/zC4vpyeFuPT0udKXuz1PfZ8nv7I+s6nzlYakF3Vm/sus59a7m29WiXl9vrxVg6BgBWmCwismDbWOoSaLsM2pW7SNsNCK08V7T72fPK4cVWztxlIdY9zipn3Ea17sil0D/6g/+z3DGbs37Plnpge8oNGq287v/NffmZz0r9XBav7c8BABhbNsXN2bF2SfNI8hSCSY+myo0K2V+tlcVLblAYJY+myuXUoXm/HL4cPErOIt7dySXNeP69uaSc/4u2DQoAwNi2lfp+VZuF5AzRtIe/Z3+2LMi+6T9oDPHw99w0kQXWR5F7Sy1os6B8rNRdtdeW2vpkIblR4+fIe6X+vJxdfKgcfVYOAGBquQy6vcxfGh3X6jK/gW5rfWRvf3AgTir1d85dryn7zrXnqWbRtdCO1lFytjH/hwAALJENkQeb61xK7i73AgAwEDmzloXakd7FG4r2TFgAgGVrwwK5s9Tl0P74JJlE9nAbV/Z6y3ft8v3EXb1nAADLSrY6WapkD7tJTFN45akR03wPAIApTFN4KdgAgGUjzz7NJcdXy2TtNvJ7bYuTPE6r24NtU/uhRTJN4aVgAwBmXhZbeR5qHqvVGrfAebvUZrh5XNeeyG3N+JelnviQZ6gupnF/ry4FGwAw07KXWhZrt5d6VNRzkQNldJ+4hWRT3bWd+6M10h1H9nzrztZl9o8Yy0JzoRlBBRsAMNNyZixf/t9ZauuLe0qdGZtEztDlWaOtPAkhzwpdCtMUXgo2AGCmZTGTBdu0nipzOz5zdu75Ug94f60szeHu0xReCjYAYKZtLKMLtq39gYGYpPDKQ+azaMyNFLub6zwWDABg5qyLHIy8GzkUeWX+40GZpGADAFhWsjXHmjL8A9knOekAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAGDl+ge0RN5wdpq0qAAAAABJRU5ErkJggg==>

[image20]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAaCAYAAACHD21cAAAAwUlEQVR4XmNgGDmAFYhnEYlrgFgIoo2BQQeIvwHxSiQFm4H4LxBPBuIQIC6Dyj8HYiWINgaGcgYkU6AgGohPA7EgmjhcjBOI16DKMTAC8XwgnoQmDgJbgZgDxEgA4gwUKQYGYyD+CsSaaOIgkI4ugAxAzvzPgOlMvADmTJBGkoAIEF9lIEMjzH9v0SXwAWRnYgtRnADZmaAAIhogOxNbVGAFPEBczwCx7QoQK6DIYgHiQHyXAaIBHYOcDXL+KBimAADIBS0leL+IwAAAAABJRU5ErkJggg==>

[image21]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADYAAAAZCAYAAAB6v90+AAABz0lEQVR4Xu2WzStEURjGX6EI+Uj52iAbpSgsbCVlIeWjlAU7FkrZkfI/EAsWVpSyJGWllI0tKyxYUMpGsfPxPPPOHccZ19x7p7mzcH71q5n33tuc55z3nDsiDocjDorhVkBXYI0+lncKYB9sgIXWtQQd8A3uy3eAD/gO1+F48hrveYSt+lheaYbnomM9g9ewy7yhFB6YBdGZ+IRrVn0YHsESqx4386ITP2DU2uGz6NgTcLV2U5eVatFgU1Z9VNLDZkMPXLaLGSiHp6IhGMaD7XgHa73CDJzzviTplvQHySKctWrZ0AKPxRhMALgNuB0YgmE8vMAcuy9cqQvRlcslRXBTtBOCwoG/in8wbpdf4exdSXob5pIx0ZULAgfObRI6mDcjdhsGpUr0B8PYCBfgiPgc2wZDEjEY9xAfjNKGPC034H0En+AN7Je/idSKPCp3RIPFST08kcyrRfwOjwrR91mvUUvh7a84g3GmD0X3WRDYSTzYXmCnUWdIhm0yagn4A6uioS6ta7miUjQU36VhaIMPot1F2GlLoi2aog7eigay5eqFeceEhftlT6L9k+Fe5L6chNuif/cmftyRRxiIp2hUyuA0HEx+djgcDsf/4gsOFmj0j6RUbwAAAABJRU5ErkJggg==>

[image22]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAC0AAAAZCAYAAACl8achAAABSUlEQVR4Xu2VsUoDQRRFr6ggRoKgaGURwUJSxkaxtBOsLAx+QD4gRYrU1oLYB0mpjaDYWIg2foA2doJgYWFlIKQw9/kcdhzc7NrMjjAHDmTmzQs3k9kdIBKJ+KZMl9zJkKnTZ3riFkJkli7QFv3EPwltyAwtv2zcGi/SKWtcBCNDr0HPzgNdoU16S3u0TSeTpV5JDb1Oz+g+dEEHScga/aDX32OXEt2mu39wg45Jcw5SQ8uX7EDDygL5bNikA/pkzfkkNbThkb7SZWuuAW26seZ8khnaHAP5y4UJ6LGRpiOzyDOZoaV4YI0r9IX2oef+N6r0Ddqb1ws6Lc05GBl6Hlo8RvKQvNMukp0vgkNorlM649S+Hrh76Nm9o+fQ117RrzrXHzsui0TZ5TnoxRI0cutd0i23EDJX0K3v0D2nFiz2bbXq1CKRiAeGGIlVJPeTHMgAAAAASUVORK5CYII=>

[image23]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADQAAAAZCAYAAAB+Sg0DAAACCklEQVR4Xu2WvytGYRTHj1DkR4lEJhYxMMgiFn+AQQYhioHNhJKYLTYDUSiDkgUpC1EMDAZGA/mRwWghP75f57lcx5v33vdF0f3Up9c9z73v+zznnuc8RCIiIv47FXAKnjuP4CycdvbA/Le7/wAlsAU+wCc46q7pMDyD9zDVe+C3yYS1NhiAZ7gM00w8B+7CeRP/cVgW4/BCNMthyBJd0JAdAGXwGs7YAZIBC+X99dnrRCmHV6L1zsmFhZNmydXbAdAhutgGO7AIL0V/+BZ2ur8pN2JYmIQ6uA8P3XWiNMETWGDibBinonsoxT/Q5wvwk4vjlxSLbjpmIAjMfr9oQkrNWKJkw224Ke+djV3uEXaJWQhh5lgKHnnwQPQ18+ZqZzwm4I3oPvnONsq3wATVmPiO6KKY+C/hg3ei+ycMfGYM5tqBJGkXrRBbbuxqjMftbr0SvMT8cCEjotmcNGPJwO7F+djSWnfxmAvi20gX7fHs9TzAPBhv813Hg+dMN1yBlfJ5ImHwyj9WgtmqGefh+gGvxLhP2BxYlzwrSBFcldjtMghcTBXcgK2iyQkKkzwgOuljM0aYdP/ZtCV6xLxmdA6uObkwfsGSaKts1PuThmXIpjEo8fcZ58DJ+mWS/Z1zwcX3RLtds2/sNZPsTF55sPN9x4Fq4UK4INZ/snBu7IDe/3UREREREX+PF0ZCZxDCX6hNAAAAAElFTkSuQmCC>

[image24]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAD8AAAAZCAYAAACGqvb0AAACCElEQVR4Xu2WwUsVURTGPxHBQCol0DQw3kJIIhGhPyBwFW7UnZt2uhACF4IR1N9Q1KKNqxLFpSZEG90Etmmh6EYCEQXBFpHu1L6PM483nhlf897jPXl5f/CD4cy9d+bOOffeAQKBwHWkiX7I6EvaZt3+Dx7SEzqPwiTP6Cl9S0fpdNTmgOasW/1zgy66WAM9p29cfIgu02YXr1uU9Y8u1gqb/JiLDyP5QSrlhQ/Ukmd0wsUG6BF94OJTdNzFKmWF3vHBEmiH7VnFUJsWH7wMZfw7rAKqzXtYRZXKfboGq1Cp6954A3IPto/9ob/pZ1i/S1EWNpEs+WoyAquALKeI9iNtwpPRtVDmX8M+gjbpx/QXnaGNUZs8gyj0S6CSP0ay5LNym94t0U76nG4j+bKeLrqAZFXmj2t9gL3oOm05qPw1Ripa0xrAD54FnQLv6G4ZHsKe+wTFUXKU+TRu0a+wMu939+JojAQqh1nYS9SSDvoFlv1/UWzy4hHs/VUdaZkXqZPPr/daTl5luARb91nI0Tmk797x0pf6MfPrWxWtMS6gwV7BOm24e9VEE9e/RiloP1qFZVnchJ0aKvenuLgByj7aDZvfT+ti6AzciRp5VQWVnMFZ+ITy/hj1AX7Qfdiv+DfaE7uvjGv/2EJhPuuuzZWj06FcNEGdFmlLII7aVPKcQCAQCATqkb+vy2yd/xXueQAAAABJRU5ErkJggg==>

[image25]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADIAAAAZCAYAAABzVH1EAAABhUlEQVR4Xu2WvyuGURTHj0SUlB8lmVhEWAx2u0hvURYbs1n5H8iikMGgxGTxDxiYxCSLxWRkUH58vx1POM/rce7z3ryp+6nPcs69z3PPe8+97yOSSCQ8NMEtp6uwU6fVhV7YboMZI/AJHsjngl/hC9yAlY8cx9zDAZ3253TBZzhlE6QVHppYA3yD6ybOB5zAFhMvy6jou4pgngVQ7gTXVbUQ7sa+iXWITlgw8VnJF1cGtscmnJPfC/lKmxQUsgiXTWwcPsAhE1+BSyYWwiA8grdw3uQ8FBZSDe7EuejOxIC/+hi8htOw8XvaTVAh3aIvtG0VChfL55yKFhHSQj8RVAjb6lHybeWFVznbhu3DVopJUCE8Axxctq2G4Q08tokIuAvh9u+KDq4FthXPQsy2Iu5CsvNRayEZk/ACnsEJkyuDqxAOWhMdeGVyseDVewlnRM9SKH2i6+PfRW5+j+jB5AArd4e7FJN+uA3vRL8qPOxJfm2Ul1Ld4SfHDmy2iUQikUj8G94B47RRPK/0LAoAAAAASUVORK5CYII=>

[image26]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACsAAAAZCAYAAACo79dmAAABbElEQVR4Xu2VvUoDQRSFr6igGPAXNWgj2FhZ2Nppa5kn8BnEZ7BR8AXUVm1EBEtBsFCwEwubIKKQVClsFNRznCzMXnd2J2wmhcwHX5G5M8uZyZ1dkUjk/3AIn2EDPsGZVDU8E3BaD7pYgzvwG57CgXQ5KJuwBbd1wUUfPICfcFXV8qjCI1jRBQ/GxJwm1/OQvMOOwztYh3PpUi5lwiZ4hx2EU3AFvsMLOJSakU9Pws7CY9iE93BfChY4CB6WffIKF62xR+m8BUjwsBzkSdr4tAA3yXC2y/BEzMZ1zfdV5AzL/nyA62o8c7KC7cJ3sS3/oQ/4klG7+l1VjDNscpHm1fiX/N2AD0HbIAlrP5yvrbqYfl2CNatWRNCww/BSTEDCXmNbcMGomP5baNd86EbYczFh9yTjzvD0ruEZvBVzSd7gDdwS8zXzpUxYniRDajfsSYQ3lfa3f0+K+fx1SpmwPYcb3oUjuhCJRCLd4Qc1SVieMuP43QAAAABJRU5ErkJggg==>

[image27]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAoAAAAaCAYAAACO5M0mAAAA4ElEQVR4Xu3RPwtBURjH8UdSjAqLSVlMBisTb0Feglcg78MoAysWgzKaKZM/g8WgFJsySOH7OPfezr3d0aL86jPc55x7nufcK/LbiaOPM/b+JX9iqOKFcWAtNLqxHSwGE8ED5eCCRlumEEUJUzHz+jLEBSsxF+hISNsCekg4zw08UfN2kAzWyFu1NHbIWrXP8Xo7OzrfTaz53MLRLTjRMbS1F3fj3KolscRBzOx1LRZxxcDbJlLBXcyn0bGaWtRbzsScoNELbcTMrC+PkHPWPsdvMcFCTJcuTmiJ+UP/fCFvVF0paG6cgKUAAAAASUVORK5CYII=>

[image28]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAAWCAYAAADNX8xBAAABLElEQVR4Xu2SvyuFURjHH/mRkrIqRZkMSrGQsmFhkLqDxWJTyl/gT5BRFsli9xcoi0FZlCxkMpDC5sfn2zm3e+7znnORxeBTn7rv85z32/Oc95r9EdpwzBd/Qid24TguuF6WfuxLnnstTFHny6ABPMI7fMBrnMFD7EjOtQyawHvcjs+aYC7WNuuHIsUgTXJpISRdQWzhtKtlg7T/iYV1FOjRC+laIhuki73BD1y16kQj7llkg7rx2EKQPMdhbE8PRUbxwsK9PeNtc9tsEd+sESafsGbVCb+NXtzAFwuBe83tMlotx7qFoH3fKFG5tIjqCtrxjRz69KWgFXzHed/IsYSPOOXqB3iFg65eRGOv4Sue4a6FOznFocax1uh/Mhl/9+CshXWW7Ref/J8qn/WdMe0DiRkcAAAAAElFTkSuQmCC>

[image29]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAkAAAAVCAYAAACUhcTwAAAAhklEQVR4XmNgGAXkAEYgFgJiViifGYh5EdIMDFeA+B0QPwLiL0D8DYi3AjE/sqIcBohJMOAGxPJIfAxgAMQ70QVhwBuIVzFA3IUVhAPxHCDmRhLzB2JJJD7DBiAWRhYAgkNALA7jmAHxYSD+AcRPgXglEJ8G4mCYAlCYIHuTgwFiBYgetAAAkQwQGeqiDKUAAAAASUVORK5CYII=>

[image30]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAUCAYAAABroNZJAAAAZUlEQVR4XmNgGAXDC7ACsRAQM6JLkAJkgHg7EIugS5ACWIB4LhDboEuQCjyAeCm6IDlAAogTGJDCxhyIQ8jAz4B4FwMUUGLIRgYKACiWEhgoiGqKA5YqUSwNxJsZKExsVEn2tAEAWXYSsYEfk2EAAAAASUVORK5CYII=>

[image31]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA0AAAAZCAYAAADqrKTxAAAA/0lEQVR4XmNgGNJAEogFkPi8QMyIxEcBMkC8CoifAPE7IL4DxPZAvBSIWZDUwYEJEL8C4glQPshkd6hYEUwRMmgA4q9AbIwmDgK+QCyNLghy72EGiJNAzkMHIE0YTgN5+iEQ/wfiBAZMD2ui8cGAA4i3MkA0gfB5IFYGYmZkRbiAFhCvAOJfDAgD/gKxK7IiXADkvHwGSMCANM5BlYYAkPOwgRwGiKaF6BIgAAodbAAkDtI0CV0CFNy4NEUD8T8g9kCXCALi90BshSa+GIhvAbE8mjgYgKxOBeJvQHwaiGcxQPxwDIgVEMoQABQPllA2NxC7MUCcFMKAGcGjYGAAAF+dKb1Xy/MPAAAAAElFTkSuQmCC>

[image32]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAYCAYAAAAcYhYyAAAA00lEQVR4Xu2RIQpCQRCGxyhq8ASCWBTB5CEsXsBjGMxewSiI2OwWo2C0GEWwiGASQez675sdWYc3Lpj3g6+8f97uzA5RIkYPzuAenuEBLuDUO4aNT3WEiVdTgkv4gkOVfVGGGzhQ34U2vMOLDkLq8AqbOvBU4Ja4G5M+cUFVBx7p1DwkWkDc4Y1+1MgorsjCvZU74KEDQUbZ6cBTgHPimrXKMsJRrM2MiPMVLKosIxzF2oxb7RHWdCCEo+RtpgtPZFzQIX4kd0CeT+J3aMkPicQ/vAEKSDOwA0DhWQAAAABJRU5ErkJggg==>

[image33]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAHYAAAAZCAYAAADkBdqeAAAFJ0lEQVR4Xu2aW6huUxTH/3KJ3C+R0EEol5KEiELI/UGKct488HDOI3KrIykUD3IpueQBuSW5FrFdkig8kHIpJJIQRbkbvz3WbI81zlxrfmp/e38n36/+7W/Nub71jTXHnGOMOc+R5syZM2c52dy0a/d3jrSZaWfN4HhsadrDtGfuqMC9d5guk7/QHB+HdaYHTTumvlXhfNN7pp9NX5q+Mn1kOlnDTrvLdK/cwZmdTJ/Jn4Xu63cv8rjp7qCL+926VEu2/JX6pg3236m+/USmyAnq24+A8bre9Hx3vWocJXcihsYQwqz7x3Rlai/guANyY8c2pgvlk4VnoMxFppflfQ+b1vS7dbDcuV+r/v1pgv1nqG8/KzGCvdF+3rfAJHhLw4tiapSQwUp4KfVFGHwMX0jtfPew1JY5xfSk6STTb6bT+92L3Ga6JDcmHtDKO7YQ7f879cGY/aS027XCzj1V7tTvTIemvsjxpj/kIbqwndzRW4e2GleZrpDP/hc68blAkfGq/DfGWE3HRvuxIdoPLftJI/vlxmnygdxQcsHYjCJM/6r+bD3S9Eu4HuIxLb30efJZf+xS92KofcW0W2irMeRY0sPu8kIv579IKQiBdz1IXlO0YOJG+xmDaD+07Mfuc3PjNOEHf1Q7nJ4jvzc6toTnFq+b9uo+UyHynRiaeM794XqImmNx6remp+RFC7mQSRjZRZ77mJgUQG/LQ+trpi807hDYX337yZk5tLbsZwHckBsjn5p+11IhwawbAmeMwUrhGaM/qKWQy73vhHYG+ptwPUTOPZ/In7Whu35DvvpbZMeW1ZMHlAIQ7d1dcw/1w7bdNWGV55AXJyGPzz7q28/EaNn/oXwMGcuNINywFSiV6Q6mn+RLPL8c19mgDNUeBjJAY7CaWdXxZYCBZsaPwYvk3LNB/iwGn9D4ojzPtoiOJTw+G64jC/J2IgHwmS3VFt11cSzPa4H9z+VG9e3HqS37FzpVHUsZnR3I/pJVc436+8jjTE+E6xolvLZWNvmX+4gSZVvD5HpEbccSFXKoixNlrSZfOdGxDCjbrJpjy/asPJffItKUwaeYo58tVIuS/zPR/hyRaix0qjr2xtzQQTgmtxCmKQZ4Iaqwo+NNFchFkziWirk2EJOsWKJBnoysHHIez3xXkxcV0bEUSvx2zbHlvnu661vk4fhqeXjGKRwakC9bYD8TJRPtZw/bgjpjQQOO5chuCMrv9aY/5aX3If3uKhQEGDc243gu91CY5JMlBjBuf2oMrUaqSqpjns2qmIT/GorLez1jOtN0rfw7Z6l+0FJjaH8a7f8+9dVgEsY8P3X4MYy7XP2Vxcym0mSPmx1aKDm6BtsOQjiOH/o+qWXo+xkG5Gn5/cVOnsuEO63c1LVRXMa6gSqWtvflR5985zrT4do4mhSi/WenvkKxv1XLAGcAtQkyNcpWgFBFOKc4IzczEI9qfFNNHyE/w0DywkXM6NqqJBSy5WhRip0itg6lCsWRbHc+lx8e4Igjur4CkS5+P4o9dqZsyaLG7OdkrQXhv7WlnArMUHIts/BEtU+ToOTKXBytNKw67Cfv5hxG3w/yyrysTv7ua3pI9ePB5YaxzKdtMw9HkrWz31mB6pncXIN0U4s4yw0rNf7DwCYDx5IX5MYZ4k35joHBxZkHmm6Vn0TdFO6bBsfIt2WbJGyrPu7+ziJUwAzwzfJikf03hQwnSNNkjXw71DoAmmkoLvhfFNvnjv8pW8n3zxwgzZkzZ86c2eVfy29BQqsviQUAAAAASUVORK5CYII=>

[image34]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA8AAAAZCAYAAADuWXTMAAAA00lEQVR4XmNgGNaAFYidgVgaXYIYEAPE/4HYF12CEBAD4isMEM1FaHIEwUkoBmleiCaHF4D8CnJyFQMZmv2AmAeIyxkgmg9A+QSBMBDvg7KDGEjQrMIAUagA5ZsC8TcgfgLEMlAxrIAFiGcBcQaSmDEQf4ViEBsnsAXinwwQZ6JjkO0gV2AFIP/sBGJXNHFJIH7IQCChgJw6lwESRchAEIhPM0A0R6PJgRUbAfF5BuzpV4IBEvIgzTORJfSB+BNUAoRB/rVEkr+IJAfDk5DkR8EwBwCnpTFO7iO2SwAAAABJRU5ErkJggg==>

[image35]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAYCAYAAADzoH0MAAAA7UlEQVR4Xu2SvQ4BURBGRygkhAiNQqOT6CS8gCfQaTQKCr0n8AKiIkqdVieiV9CoRCIalYiEUvjG3P2b3X2DPcnJTfabvXfu7BJFaCpwAc/wajzAOZwauzBjvRBGEx5hQT2PwQn8wrzKPIzgEiZ0AIYkG9R0YJGEK9jTAXk70N3ZlOGNgk+owwf86MANt88nzMgZHA/xAjswZVcGkIZbkg2Kyj18wjaMm3of/BnvRk0Jnkg276vMZkxSwKuGW1+T5Lz6yMEdSUFLZUyVZICcD1T2h6f+Jmmfr6LZkHN61h1Y9+YwzBdskPwHERE+fhXfN525yFNZAAAAAElFTkSuQmCC>

[image36]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEwAAAAZCAYAAACb1MhvAAAER0lEQVR4Xu2YXYhVVRTH/1GB0YdaUkSGk1gQFCFSEfgkQZkmUT6E1lMP+eCTUVEhGBGUkoQURBDhQ0UU9JBlYtSgEKIvCkYR9VCIYVBBUJRUtn6us5x919nn3hm5Mzlwf/Bn7t17n7v3Xnt97DPSiBGzjQtNl+fGWcRc+R7Omnmmq03n544KTPaB6YHcMYtYZfo0N06GV02/mY6bfjD9Y9phuqwcVICxdpueMp1nulP+HDpZjJsJ5pi+1sT8u3q7T/Oe6fVCj8ufg4dMi5rPA7nItM30gumKov0u06+mb0xLivbgCdMBTTxzjWm96UvTqRg0Q1xgWmv6WD434hBL6H+n6fvMdHPRR0hixL6hudB0SO5JXSE1Xz4mG4DFfGW6KrXDk2qPnwluNH1uus10zLSxt/s0j8qjpsYnjXCgKh/KN/ay2qcRcHLvq20AvKlr4v/LYPeb3pTn3lfUPtDYC1FQA2P+ZbojdwRsinxVC7cAQ74lHxvxDmvkC6zRZTB+i/CloFyZ+koIi9goz9wgD6dBcIBhjGXyNTw40a0Fcg/EE2vcavpDvv4WLIgf5CS6vAsuMY2rbbDnTbcU30tqBmOO7+S/Ra7g7+qmPeBqQo5h0STug/IKvM/0vXzD/dgrNxTgTayhDLHl8hzHnmpwkMyDF/J8D5zGj6bFuSOBJzFxaYAwIvmtRjYYm/hd7dzAZigqS5vv/8rL+8XN9/idrtDP5HHj8uc5BAxACmI/XeAQH8mNhvHOwIJY2H7TpWVHgtPHA5mUJBqEwbpOKhuMjWSPg53ydrwV+FyebvwO4wbBWnNuIhx5nkO5Sb7fQQ7CXC2DxYZR16aB3EaOY9LninbuX1wnup4tDRaHUzPY0/J2TpXTZWNU5PDc6N/QfO8H4ZpzE2mHxB/rJ7zLtFKjajBOg0Q+ru5NA9WTyY6qN0lPxcPKHJiJcRGGL8nD8hn5lQcD7pYf0CBI2LVo2SKfgwipJvOCsEvLYMDDXDD7JVLuZyyae01JGCEqWWaqIRm5h9v5PabNcq/jlWUyr2fAlaDGdXJjMQ9vIv2IfVGcqnvDINziFxVtLHCdPElTzrvYJK86Ga4EeAoLjM1ycrwVPNJ8jra/TY8VbYQ5r1SHTW/Iq+mz8mocYzJsEmP9qe5w417F/apV+RLkNwphLh5nWG36SV7GX5Mn32+btpxAMywin+q9ckOVog3YML99Ql4d+buyaQ94t8vPh3gPzLyr3jGEc82LMBSVchBUUJzo7txRghdQ9qko95nG1H2aJeSVSNZTIf4Twt8S5vxF7rWlF46Z3pYbY7rBsygS1XAcBj/Ly/UwYJHktBoUgPJaM11grC25cZhQDEiQt+eOs+QLedji7RjpetN2ecp4sRg3HYyp+x8QQ4VJjmgK/0vqA+kB42+VXzXIUeTJa8tB0wDpZY8ml4qGwgpN3NZnI1Twh3PjiBEjzkn+A0QQ9vIzEiWoAAAAAElFTkSuQmCC>

[image37]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABcAAAAZCAYAAADaILXQAAABgElEQVR4Xu2UPyhFURzHf2IglGJRRLGwGCixyODPYnlsFotNGa0GdimLLLJIVhksSjEYTBYpT8lgoBSD8uf7fb9z3z33d++t++7b9D71qXd/57zzu+d3fueK1MhBJ2zznuucVdEFj+ATfIX3cALOwwZvXsWMwBe45Z75pjMu9hNMysM6/IDDJk7mYNEGs9IKL0RLwbJYuPixDWaFh/cIf+GSxA9uAI6bWGYa4Yno4vQG9sF6f1K1DMJD+CVhom845U9KgOfUYYNpsCyrogfMBHvR4Qj98Fn0XBJhWZJYEV183w442PdMzDmLZqxMWlbG+cdtO+BguZj4Da6ZsRJsw7TF+Ta8PLN2wLEDh0Q7bdOMlSiIZratdgDvYI+JB3TDJtgCz0W7LVZebnkZfsJruCu61UvYG06LwAPfEL0fPNAr0QRMVIZ9POZ+N8Np0VIsSPwi+YzCU9EXoQ/wVipoxzRYCn7YWJYA7p51505yw68ju+cdTsJ2eCbhpeN4jf/IH9UDRJ19TAE1AAAAAElFTkSuQmCC>

[image38]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABUAAAAZCAYAAADe1WXtAAABHUlEQVR4XmNgGAWjYGgBRiAWBmIBdAlyAcjAh0D8H4rno8nVAXEwkhhBoA3E94GYFcrnBOJGIFaE8kEGZkDZ2IA0EOuiC05gwNQEsiACiMWBeA2UxgZA6lYB8UJ0CSEGhCuRwSQgTgfiBjRxZBAExP8YIBazoMlhBTuBeDMQ66BLIAFQ2J8A4gNAzIMqhR3cBeJlDPhd4MoA8fppIBZEk8MKtjHgDkuQRe1QdjkQvwViTYQ0brAeiDnQBaEA5EJQCpEE4mYg/grExigqcABQRGED/EC8AojnAvEsIN7FAIksF2RF2AAo0KPRBaEgGYgDkPggw0CG+iKJYQWeDJgBD/LqXyjuhoo1AfE7Bkgu/ALEfFBxrCASXWAUDCwAAMWYKY6gys0mAAAAAElFTkSuQmCC>

[image39]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAmwAAAA9CAYAAAAQ2DVeAAAGCUlEQVR4Xu3dX6iu2RwH8J/8afzP0EwyymiYMCUxNIWiEZO4GMpoUpO58CfKn4w7joZiksyUG400SoQa0kSIPbkgLuaGaErO1ESIKUXNTIb1td7HWXvtd++zz7H3Ofu85/Opb3s/63nOe9599+u31rNWFQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAG+HRq5wJF7a8eR78P3y+5VHzIADApkkB9YZ58JD8sA62wHpqy011sJ8JAHCkPKvleMtvWi7efuu/ntlyX8vWNH46XrXKQbu55VfzIADApkh37ZFV1nXZ0rl6T8s1841T9NiWb7Q8fr5xAK5o+es8CACwKe5peWnLv6t32Q7LR+twi6p8fv4OAICN85OWJ7U8XL3LNktn7bqWj6yuX1F9zdinW65tua22v7Bwa8tvW944jd/V8svhepFn8hm3TONPbHnMNLaXq1veNQ8CAJzrsn4t04nxqepdtozNrqzta9h+Wv3ZJ7fc2XLjajwF37L4/32rZxZ/b7ljuI4ftTzU8uGWr7X8ouXpLRe1fG94bnFZy5vmwZWstUtReMF8AwDgXJbO2bKm7JXVu2zrttzIVOPWcJ3fl2IsBVK6ZCm0/rk80Ly4epG2FFD/qD5tObq75ZLh+m/V//98r88N45Fu2+0t10/ji6dV/17pFgIAbIz7qxdeY47Xzi7buoItBdgona8HWt46JS8bRIq5uWCbpcj7TvVO3Dwd+oXq99MJXCeF2tbqJwDARkhBlGnLUbpUKdq+PI3vp2C7tLZ32CLTo8sU6bop0dlSdGVvtdGzq3cCc3+3aU9TogDAxkmBte6tyqXLNtpPwZbCbFyzFlkftxRfv2v51nBvnaVgG+VzP1m9IMsatq1a30V7QfWXFwAATsnl1btVWZv16uprvW4YHzhLxinQpfjJlOY8PZqOWDbNXa4zpZmx8ZlxmvMpLf+q/vf+qeUdw71jdfJtPVJ0/Wway9FT6bAt8n1SvM3yPZYXKAAA9iVrtzJF+LHqBcbxlh9XX9y/yTIlmb93Wbu2uKrlwWlslhcK8uboIt219w7XkanVrGUb5f/MdOhhbMoLAGyoF7X8pbafb5ktMLIdxryY/nzyutr7aKpf1+5vge4lR1NlSxAAgH07VjvXc6V4++o0dr5JsfrdeXBwb/Vp0VOV9XF7FYIAADtkcX0KttfXzqnB892FtX6vt3jcPLAPWeM2djIBAPbl3XViUX4W4TsyCQDgCErX5zPVXzZI4ZaD1S8eHxik63SyLlHeMM1i/pNlr33IPn4e5eUFALCL+ZSAWDakXXcOZvY4y55meQYAgDNg3dFJ2ets3XYUcWvL92v93mKjg+iwAQCc957b8sfaOb15U/UtLWYXVT8JIGvc1p06AADAAbum+tTnjdU7YpHi7eHVz9kHVj8zVXr1eAMAgMPxluods2zlkaOobml57bYnTshU6FdavthyZ517b5K+pLYfSzV6YcsjLfe0PK/lkpbft7y9+ua4AADnhKW7Ftksdrfi5yjKmrwf1PrvnKOkHqpeqI5dxby1+UCd/AB4AICz7pvVC5qvtzyh+gHpf16NjYecH2U5YiuZC7Z0GP/Qctk0vkgXcdPPUgUAOOtywHoKsztqZ8GW81OzafBuslbvGfMgAAAHJ4fa3736fS7Yrqid56cCAHCGfalOnI06F2y5vn+4BgDgDMu6tOcM12PBlpcQtlaZ5S3YMXnBYpECL2etXrq6fs1q7N5avwExAAB7uK9OHGg/J26v9QVb5ISH7EU3v3CQveduaPl59e1Q4sr/3QUA4LQtHbVxSvS66gfdr3N99XvzOavvr37CQ7ps167G3nniNgAApyNr2C6vvinuzbX9DNTss/bB1TOLT1Tvrn1oGFvk32evtmMtD1Z/g/Sz4wMAAJy6dMTWTYnG81fX2VMu69W+3XJb9ULsquG5xdtWP/OGaYq9l1XvugEAcARcUNv3ZEtBlxcOcowVAABHQM4YHY+uyoa8d1Uv5AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAOGj/AXk0EPbC/KoPAAAAAElFTkSuQmCC>

[image40]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAB0AAAAZCAYAAADNAiUZAAABpklEQVR4Xu2UsStHURTHj1BESSTK8GNTZEBhUfIHIIVkMbOSTclmNKFksEkZ1E8WGSTKIINkQLIYlEFR4vvt3Ptz3fd+T3nvl+V961Ovc+97557vPeeJpPpHFYEa0ODFS0GFF4stJtsDH+ATPIIjkAHlYB1M2M1JqB7sgF3QBopNfAicg33wAtpNPJY6wRN4Br3emlUXeBWtNBGdilo5K2pvmHi3d5KgtUx4Cer8BUdMysO1+At/UZNo0jl/wROTjog2U2xtgjNQ7S8USpXgEGxJ8C7ZubSbFbrwHVfj4MFA16xs7BosOfFcUlbriyNzAe5F7bczO+luMmoGb2DaifGAaxI8pJSAbQlP6ooJNyTohtUAyIITUGViHLH53A5PbCC+kK9BeNdMGjUqM2BM9C82bGJToofJK26mjd3ys5qM6JhENVojWDTPC6I294BlUGbioeoDN6IV3YJV0URXoF++PxomVjNqnltF/2orotX/KnYrB5+zOChaZb47dMWPd5hn7mdCdm2ktXFE+2hjrROjtbSYtieuA/Au2g/H3hqbKlWqwukLbn1MDZnXKeAAAAAASUVORK5CYII=>

[image41]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABMAAAAYCAYAAAAYl8YPAAAAxUlEQVR4Xu2RIQpCQRRFn6CgaFIRRGwWN2AzCoLRBbgBu7switjMBoNgtVjchsFt6L3MIPzLzP+afpkDp8y9D+bNmCUS5dCAWzjUwDMyl9c1CLGBaz0UmLOXywReYUcDoQdv5vpBxvBhOQWBvbu5tTM04RMuYP8Pl36O7/xlBd/w5cNfZZ9znM+wg3tY0yACtzma+9kgLXiGUw2EGTyZrBdiDg+wooGnau5G7BXShRc40MDDc+bsFcIbtS3+djxnHrt5oiw+CCUhbqgbKHQAAAAASUVORK5CYII=>

[image42]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEgAAAAZCAYAAACSP2gVAAAD9ElEQVR4Xu2YXaiOWRTHl1Dk28hHyDGhlJKEFDcoDCONuZi4US4orkwIKZLyEU0TJXHhYkaaqVHozIWLkylEaRQpUUgjyoiauTDjY/1az+rss579eM9x3l7n4v3Vv/e8a+/n2Xuvvdba+7wiTZr0NPqqhkdjD4W5DonGrjJUNUbVOzZkYLDfVKtiQw+F+f6k2hQbOsMx1WvVX6rHqreqH1WD004JDNaq2q7qpVok9hx6k/RrBP1Up1Qngs6pxif94AvVVbE5d4r+qkOq/WIPO4tVL1X3VJMSu7NVdU3anxmrWqO6o3rvnRpEH9W3qstiY7NJfF8ollaR+arZ0RgZp7ohFilVKTJMrE9cMN6/qxoV7LBNyv0bwVTVC9U7sWiuBVG+JBpTzost5AepDjd25lcpL5hoIf1yfC4HrRAb96HY/GpBpJ8RW2MWXka9yaWPg+MoavQlzx0m803yPaXKQbyLdOQAGBnaUkgJj0yemSKWLrVgwxiXDa1cdALreigVzmQCvOyoVEcPDFS1SdlB+1TTk+8pOQcxxgOxd1E8+Vxe2B2uCuzov2I15LrYCUldeaQa0d41i5cCxu8M9PtPNS82AN5+qvoyNgQ8bNMFu9OoTzmig2aq/hE7DFJ+FzsEZhTfqR2XVAOK7/6eqlSO0Je0qeVIhzrFmCWHMgEm8odqUGhLYXeJMAZ+ktjdQXzmiA7y0I+cFrMTjRDTw99Dv1owV/qSNrmMwBbvdb5xJQf5AlHVIoHaRI1i4L2JnfsPx3vVs6mDfDNyDtohZr8olr5EE2nikentG4rvH4Oooe/62FAwTco36EoHeeFtk+pFAqcbg96WjkW1KxGU1rCI9/O0OiwW8jvFriA4rFXKC8vBYqlds2JDwe5oEOvLMyUHAcZa+cr9iEnGC5UvelSwO11NMa8xF1RfqXaJRdUyKadFFURO1XrIhJvRqHwtNv7m2ODgAG7JExIbE1otFnocr1Xw0lz154gmEhjYF0fEcuteV/zttv9V3yc20pbL25/S/m/DHrHTMldXADvtlIK1iZ2U3ah6JTYXDpsItY+LJRfMLByzz8XC7LjYA/cLG/8yfIy5Us5335FU2ICF8O5nYqcXn0sLu7NFys+7fkn6OSel3C+nu5KP9jaxucTTtQPsMvn7nWqlqkWqdyuFuuDFtSv4LwV8pjDm32JRmUZZi+pnsdpUb4ieTdFYTxiA06EesMPUpBwU7PSaUS9458RorCcUb27Hc2LDJ3JFLA2JZpwyWXVErAQcSPp1FyKTn2g6czp2G34FuCUdC/2nQrrj7INiR/9ZsToXf8/pLsyZ+1bDWCDtt+GeDv9aUdxHx4YmTZo0hA/U0uwVwnEeSgAAAABJRU5ErkJggg==>

[image43]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAcAAAAbCAYAAACwRpUzAAAAkElEQVR4XmNgGAJABV0ABhSBeCG6IAx4AnE5uiAMtAKxC7ogCHAA8VYglkYW5AFiSSCOAOJ/ULYYEDMjKwLZ9R9ZAAZYgHgNED9HlwABcSC+C8QH0MTBwAaIfwPxJHQJEChigNgXxACxAuQ4YZAEzL63QKwJxMZAvBiIOcHagMAXiD8C8QYGSChhAJh/RxwAAAqIErJPedn0AAAAAElFTkSuQmCC>

[image44]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADIAAAAZCAYAAABzVH1EAAABg0lEQVR4Xu2VTysGURTGH0URKf+SrNiJHV9DShZKSjbslIWV8gFsRDZKsrBQtj6DhZ1Y2khkYclC+fM8HROdGdPcmXkp3V/9Nufemfee95xzB4hEIkVooXsFXafd9tifMEA7fTBhjD7TY3wd+I2+0h0687mmPfd02B77dXroC530C6KNnrhYE32n2y6uF5zSVhf/jqo1CntHHeg9SkCqEjpXZiKqxpGLdcEemHPxaaST8/TRfXoBa9k66UBOIgt02cXG6SMdcfFVuuRiPzFE7+girOp1kJtIFqrEOawyVVA7bNJbuubWyhCUSC+9Qrqt6mCFPtBd2O0TSlAiaqsnpNuqLtRmaje1ndovhKBENAPaXLWt8tAlME+3aLNby6NwIrrqDmCbG0FSjRvYzRZK4USS+WhEIu2wodfw6xIoQ6FEtGkDtvHSrZVFQ61/X0OuRKoyCDufPhepb1Q/vYZt8Ko6qlIoGmK16CwyfrAEh0ifTepSahgT9IxO+YVIJBKJ/Ds+AAsUUcQejPUQAAAAAElFTkSuQmCC>