FORMATION DEVELOPPEUR WEB - OPEN CLASSROOMS - PROJET 2 - FABIAN DENEUVILLE

TRANSFORMER UNE MAQUETTE EN SITE WEB AVEC HTML ET CSS
<hr>

<b>Spécificités fonctionnelles comme énoncées dans le briefing et en gras, les réponses apportées/solutions adoptées :</b>

- Les usagers pourront rechercher des hébergements dans la ville de leur choix. Le champ de recherche est un champ de saisie, le texte doit donc pouvoir être édité par l'utilisateur. Il faut englober ce champ dans un formulaire pour que ce dernier soit valide auprès du W3C. La partie recherche ne doit pas être fonctionnelle.<br>

<b> -> Création d'un formulaire (attribut action non renseignée car le formulaire ne doit pas être fonctionnel) avec un champ de type search, éditable par l'utilisateur. </b>

- Chaque carte d'hébergement ou d'activité devra être cliquable dans son intégralité (pas uniquement le titre). Pour l'instant, les liens sont vides. On peut utiliser un attribut 'href="#"' pour simuler la présence d'un lien. <br>
  
<b> -> Chaque carte est un lien, les cartes sont donc cliquables dans leur intégralité.</b>

- Les filtres doivent changer d'apparence au survol. Je te laisse décider de l'effet approprié, je n'ai pas encore eu le temps de me pencher dessus. Par contre, ils ne doivent pas être fonctionnels.<br>

<b> -> Ajout d'un box-shaddow et changement de la couleur du texte au survol. Lien simulé avec un attribut 'href="#"'.</b> 
  
- Les textes "Hébergements" et "Activités", situés dans l'en-tête, sont des liens. Ils doivent mener respectivement vers la section "Hébergements à Marseille" et "Activités à Marseille". <br>

<b> -> Attribution d'un "id" aux sections "Hébergement" et "Activités" pour créer deux ancres. Les liens du header renvoient vers les deux sections.</b>

<hr>

<b>Spécifications techniques comme énoncées dans le briefing et en gras, les réponses apportés/solutions adoptées :</b>

- Deux maquettes ont été réalisées : l'une desktop et l'autre mobile. Le site devra être également adapté aux formats tablette. Pour les tablettes, nous sommes libres de faire les adaptations nécessaires. Il est important qu'aucun élément ne soit oupé; et que le texte ait une taille suffisante.

- Concernant les breakpoints, nous avons convenu avec le client d'utiliser 992px et 768px. 992px pour les écrans d'ordinateurs et 768px pour les tablettes et tout ce qui est en dessous de 768px pour les téléphones portables.

- Il faut d'abord réaliser l'intégration pour les ordinateurs (autrement dit, en desktop first), puis les tablettes et enfin les téléphones. L'utilisation des Media Queries nous prmettra de réaliser l'intégration pour les différents supports.

- Plusieurs formats et tailles d'images ont été exportés. Ill faudra vhoisir le format le plus adapté par rapport à la résolution et au temps de chargement.

- Les icônes proviennent de la bibliothèque Font Awesome. Nous pouvons passer un CDN pour faciliter le chargement des icônes.

- Les couleurs de la charte sont le bleu (#0065FC), une version plus claire de ce bleu (#DEEBFF) et le gris pour le fond (#F2F2F2).

- La police du site est Raleway. Nous pouvons passer par Google Font pour importer facilement cette police dans ke code : https://fonts.google.com/specimen/Raleway.

- Il est important d'utiliser les piwels et les pourcentages plutôt que les REM et les EM. Le client préfère cette solution pour des contraintes techniques.

- Il est important d'utiliser Flexbox plutôt que Grid. Notre client est plus à l'aise avec cette solution.

- Aucun framework CSS (type BootStrap ou Tailwind CSS) ou préprocesseur CSS (type Sass ou Less) ne doit être utilisé.

- Il est important d'utiliser des balises sémantiques (type 'main', 'header', 'nav', etc.).

- Le code doit être valide aux validateurs W3C HTML et CSS.

- La maquette doit être compatible avec les dernières versions de Google Chrome et Mozilla Firefox. Il faudra tester le prototype sur ces deux navigateurs.

- Le code ne doit pas être versionné avec Git.

