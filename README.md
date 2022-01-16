FORMATION DEVELOPPEUR WEB - OPEN CLASSROOMS - PROJET 2 - FABIAN DENEUVILLE

TRANSFORMER UNE MAQUETTE EN SITE WEB AVEC HTML ET CSS
<hr>
<b>CONTEXTE : </b>

Durant un premier stage en tant que développeur web chez Booki, une petite entreprise proposant un outil de planification de vacances nous sommes solicités pour travailler sur le prototype de la homepage que nous devons intégrer en respectant deux maquettes (une desktop et une mobile) et en observant les spécificités fonctionnelles et techniques suivantes.

<hr>
<b>SPECIFICITES FONCTIONNELLES COMME ENONCÉES DANS LE BRIEFING ET EN GRAS, LES REPONSES APPORTÉES/SOLUTIONS ADOPTÉES :</b>

- Les usagers pourront rechercher des hébergements dans la ville de leur choix. Le champ de recherche est un champ de saisie, le texte doit donc pouvoir être édité par l'utilisateur. Il faut englober ce champ dans un formulaire pour que ce dernier soit valide auprès du W3C. La partie recherche ne doit pas être fonctionnelle.

<b> ⇒ Création d'un formulaire (attribut action non renseigné car le formulaire ne doit pas être fonctionnel) avec un champ de type search, éditable par l'utilisateur. </b>

- Chaque carte d'hébergement ou d'activité devra être cliquable dans son intégralité (pas uniquement le titre). Pour l'instant, les liens sont vides. On peut utiliser un attribut 'href="#"' pour simuler la présence d'un lien. 
  
<b> ⇒ Chaque carte est un lien, les cartes sont donc cliquables dans leur intégralité.</b>

- Les filtres doivent changer d'apparence au survol. Je te laisse décider de l'effet approprié, je n'ai pas encore eu le temps de me pencher dessus. Par contre, ils ne doivent pas être fonctionnels.

<b> ⇒ Ajout d'un box-shaddow et changement de la couleur du texte au survol. Lien simulé avec un attribut 'href="#"'.</b> 
  
- Les textes "Hébergements" et "Activités", situés dans l'en-tête, sont des liens. Ils doivent mener respectivement vers la section "Hébergements à Marseille" et "Activités à Marseille".

<b> ⇒ Attribution d'un "id" à l'article listant les hôtels dans la section "Hébergement" et à la section "Activités" pour créer deux ancres. Les liens du header renvoient vers les deux éléments.</b>

<hr>

<b>SPECIFICITES TECHNIQUES COMME ENONCÉES DANS LE BRIEFING ET EN GRAS, LES REPONSES APPORTÉES/SOLUTIONS ADOPTÉES :</b>

- Deux maquettes ont été réalisées : l'une desktop et l'autre mobile. Le site devra être également adapté aux formats tablette. Pour les tablettes, nous sommes libres de faire les adaptations nécessaires. Il est important qu'aucun élément ne soit coupé; et que le texte ait une taille suffisante.

<b> ⇒ Intégration du site et des différentes section sur Desktop puis utilisation des media queries associés à Flexbox en CSS pour adapter d'abord le design sur tablette puis sur mobile. </b>
  
- Concernant les breakpoints, nous avons convenu avec le client d'utiliser 992px et 768px. 992px pour les écrans d'ordinateurs et 768px pour les tablettes et tout ce qui est en dessous de 768px pour les téléphones portables.

<b>Les deux breakpoints de 992px et 768px imposés ont été respectés. J'ai ajouté un autre breakpoint à 1500px pour les écran d'ordinateurs portables et deux autres breakpoints à 450px et 350px pour afficher la barre de recherche de manière optimale sur tous les appareils mobiles.</b>

- Il faut d'abord réaliser l'intégration pour les ordinateurs (autrement dit, en desktop first), puis les tablettes et enfin les téléphones. L'utilisation des Media Queries nous permettra de réaliser l'intégration pour les différents supports.

<b> ⇒ Intégration du site et des différentes section sur Desktop puis utilisation des media queries en CSS pour adapter d'abord le design sur tablette puis sur mobile. </b>

- Plusieurs formats et tailles d'images ont été exportés. Il faudra choisir le format le plus adapté par rapport à la résolution et au temps de chargement.

<b> ⇒ Utilisation des images ayant les dimensions les plus petites pour la section hébergement car leur taille est suffisante. Utilisation des tailles de fichier large/medium/small pour les activités avec les attributs srcset et sizes pour permettre au navigateur de choisir le fichier adéquat selon l'appareil utilisé et sa largeur d'ecran.</b>

- Les icônes proviennent de la bibliothèque Font Awesome. Nous pouvons passer un CDN pour faciliter le chargement des icônes.

<b> ⇒ Import de la bibliothèque Font Awesome dans l'élément Head du fichier HTML.</b>

- Les couleurs de la charte sont le bleu (#0065FC), une version plus claire de ce bleu (#DEEBFF) et le gris pour le fond (#F2F2F2).

<b> ⇒ Les trois couleurs ont été utilisées. </b>

- La police du site est Raleway. Nous pouvons passer par Google Font pour importer facilement cette police dans le code : https://fonts.google.com/specimen/Raleway.

<b> ⇒ Import de la police dans l'élément Head du fichier HTML. Raleway étant la seule police utilisée par défaut sur le site, celle-ci est définie pour tous les sélecteurs dans le fichier css, en plus des polices Arial, Helvetica et Sans-Serif, dans le cas où la connexion avec la bibliothèque Google devait rencontrer un problème.</b>

- Il est important d'utiliser les pixels et les pourcentages plutôt que les REM et les EM. Le client préfère cette solution pour des contraintes techniques.

<b> ⇒ Seuls les pixels et les pourcentages ont été utilisés pour définir les dimensions, marges et paddings du site.</b>

- Il est important d'utiliser Flexbox plutôt que Grid. Notre client est plus à l'aise avec cette solution.

<b> ⇒ Utilisation exclusive de Flexbox.</b>

- Aucun framework CSS (type BootStrap ou Tailwind CSS) ou préprocesseur CSS (type Sass ou Less) ne doit être utilisé.

<b> ⇒ Aucun framework ou préprocesseur CSS n'a été utilisé.</b>

- Il est important d'utiliser des balises sémantiques (type 'main', 'header', 'nav', etc.).

<b> ⇒ Les balises sémantiques ont été utilisées à chaque fois que cela était possible. Un Header, un Footer et un Main regroupant une section Search, une section "Hébergements" contenant un article et un aside et enfin une troisième section "Activités".</b>

- Le code doit être valide aux validateurs W3C HTML et CSS.

<b> ⇒ Les deux fichiers HTML et CSS ont été passés au validateur W3C. Une alerte côté HTML concernant l'absence de titres pour la section hébergements mais ceux-ci sont présents dans les éléments enfants. </b>

- La maquette doit être compatible avec les dernières versions de Google Chrome et Mozilla Firefox. Il faudra tester le prototype sur ces deux navigateurs.

<b> ⇒ Le site a été testé sur les deux navigateurs à chaque étape de l'integration. Je me suis par ailleurs assuré de n'utiliser que des fonctionnalités supportées par les dernières versions des navigateur grâce au site caniuse.com. Concernant l'utilisation des attributs srcset et sizes pour les images, en cas d'incompatibilité, l'attribut src a été renseigné.</b>

- Le code ne doit pas être versionné avec Git.

<b> ⇒ Les fichiers envoyés pour la soutenance et qui feront l'objet de l'évaluation n'auront pas été versionnés. Les fichiers présents dans ce repository ne sont qu'une copie faite par souci de sauvegarde, pour m'exercer à l'utilisation de Git et GitHub et pour pouvoir présenter mon travail autrement qu'en envoyant mes fichiers.</b>

<hr>

<b>RESULTAT : </b>

![booki](https://user-images.githubusercontent.com/94392055/148818049-f8f5b147-5c25-40d8-bd34-413ae0bd725d.png)
