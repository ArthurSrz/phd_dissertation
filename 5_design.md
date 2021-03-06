# Design d'un `dispositif en Système d'Information` permettant de résoudre les situations problématiques qui freinent l'usage des données ouvertes


Dans le chapitre précédent...

Dans ce cinquième chapitre, il est question de passer des besoins fonctionnels au design d'un prototype qui permet de répondre à la situation problématique. Le design d'un prototype est constitué de trois éléments : 
  1. Des éléments fonctionnels identifiés à partir des besoins fonctionnels et qui assurent la transformation de la situation problématique en situation désirée. On parle de **proposition de design**
  2. Des mécanismes issus de *kernel theories* qui expliquent en quoi les éléments fonctionnels permettant le passage de la situation problématique à la situation désirée. On parle de **principes de design**
  3. Un modèle conceptuel qui dessine l'architecture de l'artefact, intègre les éléments fonctionnels et explique les fonctions qu'il assurera dans un contexte réel. On parle également du **design du système** que consitue l'artefact.

### Construction des propositions de design

Pour pouvoir construire les propositions de design, nous avons conduit une nouvelle revue de la littérature visant à identifier des éléments fonctionnels qui puissent répondre aux 12 besoins fonctionnels identifiés dans le [chapitre précédent](4.1.4_connaissance_resultats_discussion.md).Précisons que cette revue de littérature vient compléter celle présentée au [chapitre 2](1.0_revue_de_litterature.md) en ce qu'elle vise à identitifer des articles et atteindre des résultats complémentaires.

Nous ne reviendrons pas sur l'approche complète de la revue de littérature détaillée dans le [chapitre 3](2.2.2_design_recherche_méthodes.md) mais précisons les aspects méthodologiques qui diffèrent entre la première revue de littérature du [chapitre 2](1.0_revue_de_litterature.md). 

Ces différences ont pour origine des inspirations différentes. Alors que la méthodologie de la première s'inspirait des travaux de Bogers et al.(2016), fixant des règles pour mener une littérature classée selon des niveaux d'analyse, celle-ci se base sur les travaux de Tranfield, Denyer et Smart (2003) et de Denyer, Tranfield et Van Aken (2008). Ces auteurs proposent une méthodologie de revue de littérature visant à contrecarrer le manque de pertinence empirique des revues de littératures dites traditionnelles. L'objectif de cette méthodologie est de permettre au chercheur d'extraire de la littérature des éléments qui puissent informer et guider les praticiens dans la réponse à apporter à leurs besoins opérationnels. Ces éléments sont des **propositions de design**. 

Elles empruntent leur logique à la règle technologique de Bunge (1967), qui se formule ainsi : `étant donné le contexte empirique C pour résoudre le problème P et dans l'objectif d'atteindre l'objectif O, alors utiliser l'intervention I`. Cette logique a été créée initialement pour cadrer la manière de formuler des connaissances prescriptives en matière de résolution de problème à travers l'implantation d'une technologie. Je la réutilise pour formuler des propositions de design qui viennent toutes répondre à une dimension de notre problématique de recherche. 

Dans toutes les propositions de design, les `contextes C` correspondent au contexte de l'usage des données ouvertes dépeint au [chapitre 4](3.1.3_explo_connaissance_formation.md) et les `problèmes P` aux barrières qui freinent l'usage des données ouvertes. L'`objectif O` de chaque proposition est evidemment de lever une ou plusieurs barrières freinant aujourd'hui l'usage des données ouvertes. Enfin, l'identification de `l'intervention I` est le résultat de notre revue de littérature et sera annoncé à la fin de la première section de ce chapitre.

En premier lieu, et contrairement à la première revue de littérature, celle-ci n'a pas été structurée sur la base d'une liste de concepts visant à décrire un phénomène. Plutôt, cette revue de littérature a été réalisée en suivant la structure des 5 étapes d'usage des données ouvertes construites au [chapitre 4](3.1.3_explo_connaissance_formation.md). Ainsi, des recherches distinctes ont été menées de manière à ce que les articles identifiés correspondent à chacune de ces 5 étapes. Nous obtenons ainsi cinq corpus d'articles correspondant aux cinq étapes d'usage
Aussi, dans chacun des 5 corpus d'articles, la revue de  littérature s'est-elle développée sur la base des [12 besoins fonctionnels](4.1.4_connaissance_resultats_discussion.md) qui apparaissent au cours de ces 5 étapes. Par là, il est question d'identifier dans la littérature des éléments fonctionnels qui puissent répondre à ces besoins. 

En second lieu, et contrairement à la première revue de littérature, celle-ci n'adopte pas le niveau d'analyse comme critère de sélection des articles. Plutôt, cette revue de littérature sélectionne les articles sur la base des trois critères suivants : 

- cohérence entre la problématique de recherche adresée par l'article d'une part et un ou plusieurs des 12 besoins fonctionnels d'autre part.
- cohérence et similitude entre le contexte empirique auquel répond l'article d'une part et le contexte propre à l'usage des données ouvertes tel que décrit au [chapitre 4](3.1.3_explo_connaissance_formation.md) d'autre part. 
- l'article contient une description suffisante de l'élément fonctionnel qu'il propose pour répondre à sa problématique et fait référence à des travaux de recherche qui se sont attachés à le décrire et comprendre ses mécanismes sous-jacents. 


Enfin, cette revue de littérature a été menée sur la base d'une liste de mots-clés venant compléter celle utilisée pour réaliser la première revue de littérautre. Cette liste, que nous présenterons dans ce chapitre, a permis d'orienter clairement la recherche d'articles de manière à identifier des articles en lien avec les 12 besoins fonctionnels. Ces mots-clés ont permis d'effectuer des recherches sur plusieurs bases de données (Crossref, Google Scholar, Microsoft Academic et Scopus) et nous a permis d'obtenir de riches corpus d'articles. 



### Construction des principes de design

Les principes de design précisent les propositions mentionnées ci-dessus. 

Pour construire les principes de design, nous avons orienté la revue de littérature dans une nouvelle direction : la recherche de _kernel theories_. Ces kernel theories jouent le rôle de "noyau" théorique autour duquel nous construirons le design de l'artefact, résultat final de cette thèse. Hanseth et Lyytinen (2004) les définissent comme "les théories issues des sciences naturelles et sociales qui gouvernent les exigences de conception ou le processus qui permet de les construire". Bharosa (2011) précise que ces théories acquièrent un caractère opérationnel par leur traduction en "lignes directrices et normatives, formulées de façon à permettre aux architectes de système d'information d'agir" (Bharosa, 2011, p.118), autrement nommées **principes de design**.

Ils prennent la forme de la logique "PIMCO" (Carlsson, 2006), qui se formule ainsi : ` étant donné le contexte théorique C(t), pour résoudre la classe de problème P, il est pertinent de mettre en oeuvre l’intervention I dans la mesure où elle déclenchera les mécanismes naturels, sociaux ou techniques M, moteurs pour atteindre l’objectif O`. Dans tous les principes de design, le contexte théorique `C(t)` correspond à la vision d'un phénomène dictée par la _kernel theory_ sous-jacente à chacun des trois éléments fonctionnels (le réseau d'information, l'infrastructure, le manifeste et son codebook). Pour leur part, la classe de problème `P` correspond à un type de problème traité par la _kernel theory_, l'intervention `I` à un des trois éléments fonctionnels. Enfin, les mécanismes naturels, sociaux ou techniques `M` correspondent aux élements médiateurs, tirés des _kernel theories_ et qui assurent le lien de cause à effet entre l'intervention `I` et l'atteinte des objectifs `O`, à savoir lever les barrières relatives aux cinq étapes. 

A propos des _kernel theories_, précisons dès à présent que dans cette thèse, nous partons, avec Gregor (2006), du postulat que des théories peuvent parfaitement acquérir un caractère normatif et directif. Dans son article majeur sur la théorie du design, Gregor (2006) établit qu'il existe 5 types de théories interdépendantes : les théories pour analyser (1), les théories pour expliquer (2), les théories pour prédire (3), les théories pour expliquer et prédire (4), et les théorie pour agir et designer dites (5). Ces théories ne s'opposent pas. Elles se complètent. En l'espèce, les _kernel theories_, choisies parmi les quatre premiers types de théories, "informent" le cinquième type : les théories pour agir et designer (Carlsson, 2006, p.222). Pour faciliter sa compréhension de cette relation entre théories, le lecteur pourra considérer que les _kernel theories_ sont un noyau théorique duquel une lecture "orientée pratique" permet d'extraire un design et/ou une théorie du design

Si les _kernel theories_ sont issues d'une lecture "orientée pratique" des quatre autres types de théories, il s'agit pour les identifier d'approfondir la revue de littérature mentionnée dans la section précédente. Pour cela, nous avons repris les mêmes articles, en cherchant les références théoriques qui pouvaient nous orienter vers des _kernel theories_. Une fois ces _kernel theories_ identifiées, nous avons rajouté leur nom à la liste des mots-clés utilisés pour effectuer nos recherches dans les bases de données (Crossref, Google Scholar, Microsoft Academic et Scopus). De ces recherches nous avons extrait des articles délimitant le champ des courants de littérature associées aux _kernel theories_. 

Finalement nous avons analysé ces articles en cherchant à extraire les configurations PIMCO (_Problem, IS Initiative, Mechanisms, Context, Outcome_) décrites par Carlsson (2006). Il s'agit d'extraire la classe de problèmes adressée par la théorie (_Problem_) ; l'intervention en Système d'Information évoquée dans la théorie pour le résoudre (_IS Initiative_) ;  les mécanismes sociaux, naturels ou techniques qui justifient le changement opéré par l'intervention (_Mechanisms_) ; le contexte de mise en oeuvre de cette intervention (_Context_) ainsi les résultats escomptés (_Outcome_).  


### Construction du design de l'artefact 
Sur la base des 12 principes de design, nous avons designé un `dispositif en système d'information` visant à faciliter l'usage des données ouvertes. Tous les principes ont été incorporés dans le design. 

Pour rappel, au regard du modèle théorique développé au [chapitre 3](3.1.3_explo_connaissance_formation.md), le `dispositif en système d'information` que nous avons décidé de designer est un environnement de conception des usages des données ouvertes dit artefact de meta-design (Fischer et Giaccardi, 2006). Un artefact de meta-design se définit comme "une infrastructure technique et sociale dans laquelle de nouvelles formes de design collaboratifs peuvent prendre forme. Il dépasse la notion traditionnelle d'artefact en ce qu'il intègre un processus co-adptatif entre l'artefact et l'utilisateur, élevant ainsi l'utilisateur au rang de co-développeur ou de co-designer de l'artefact" (Fischer et Giaccardi, 2006, p.1). 

On distingue quatre caractéristiques chez les artefacts de meta-design(Giaccardi, 2003, p.156) : son habitabilité, traduite par un espace électronique dans lequel l'utilisateur peut vivre et avec lequel il peut interagir ; un paramètre relationnel, traduit par le fait que la forme de l'espace électronique peut être négocié entre individus, en relation avec la technologie. ; sa co-évolutivité mise à disposition par des interactions réciproque et récursive entre l'artefact et l'utilisateur, laissant ainsi transparaitre le caractère "ouvert" de l'artefact ; et enfin sa convivialité mise en oeuvre par la possibilité offerte par l'artefact de faciliter sa gouvernance par une communauté. 

Dans cette partie, il s'agit de construire le design du système que constitue l'artefact de meta-design. Le design d'un système décrit la structure et le comportement de ce système (Offermann et al., 2010). Nous commencerons par décrire la structure et le comportement de l'artefact de meta-design dans son ensemble avant de nous tourner vers les 3 élements fonctionnels : le réseau d'information, l'infrastructure basée sur un modèle de méta-données et la manifeste associée à son codebook (voir Figure ci-dessous)

![](http://opendatatales.com/wp-content/uploads/2020/07/Figures-graphiques-3.png)
##### Figure : Design du système de l'environnement de conception des usages et des trois éléments fonctionnels

Ensuite, nous préciserons les pattern de coordination. Ces pattern définissent les parties réutilisables d'un design, leurs apports et comment ils peuvent être appliqués dans un contexte réel, ainsi que les relations qu'entretiennent les différentes parties du design entre elles (Offermann et al., 2010). La figure ci-dessous représente ces pattern de coordination sous forme de flèches colorées. Nous avons fait le choix de présenter ces pattern de coordination sous la forme de scénario d'usage, c'est à dire sous une forme narrative "qui décrit la situation dans laquelle l'usage de l'outil en cours de conception, va se construire et prendre sens"(Pascal et Rouby, 2006). Pour construire ce scénario, nous utiliserons le modèle de scénario d'usage proposé par Pascal et Rouby (2006).

Cette approche possède une double utilité pour le chercheur-concepteur que je suis. La première utilité tient au fait qu'elle offre une aide substantielle pour m'aider à concevoir un environnement de conception des usages des données qui soit compatible avec l'environnement et le quotidien de ses futurs utilisateurs, que l'on designera comme "système fonctionnel d'accueil" (Pascal et Rouby, 2006, p.3). En d'autres termes, cette approche prête au scénario d'usage la qualité trés utile de renforcer la coordination de mon artefact avec le contexte réel de ses futurs utilisateurs. Pour cela, le scénario d'usage viendra peupler les items suivants tirés des données récoltées pour l'étude de cas présentée au [chapitre 4](4.0_etude_de_cas.md) : 

- [ ] mentionner ici le travail à l'échelle nationale avec Datactivist X FING ?

- Caractéristiques de l'utilisateur de l'artefact : identification, statut, rôle, caractéristiques personnelles susceptibles d'impacter ses attentes concernant l'artefact (formation, expérience ...).
- Tâches réalisées à l'aide de l'artefact et type de déroulement (séquentiel, itératif, en parallèle) : voir section précedente
- Les partenaires qui prendront part à la réalisation des tâches
- Les ressources qui seront mobilisées pour réaliser les tâches
- Les informations et flux d'informations nécessaires pour réaliser les tâches
- Les outputs des tâches réalisées

La deuxième utilité tient au fait qu'elle propose une aide pour m'aider à intégrer l'artefact dans l'environnement structurel de réference des usages (ensemble de règles et ressources). En d'autres termes, l'approche de cognitivo-structurationniste prête au scénario d'usage la qualité de renforcer la coordination de mon artefact avec le contexte structurel, (evidemment plus large que le contexte quotidien des futurs utilisateurs) des grandes logiques d'action sollicitées par les acteurs et organisations impliquées dans le développement des usages des données ouvertes. Pour cela, le scénario d'usage viendra peupler les items suivants tirés des données récoltées pour l'étude de cas présentée au [chapitre 4](4.0_etude_de_cas.md) : 

- Les schémes interprétatifs utilisés pour guider les actes des individus (modes de raisonnement, cadres de référence ou représentation collective). Ces schémes sont compris ici comme les enjeux, contours et contenus du procesuss entourant les tâches réalisées par les acteurs
- les normes qui jusitifient et légitiment les actes, comprises comme moyen d'assignation de rôles et de devoirs aux utilisateurs de l'artefact et à leurs partenaires
- les facilités, comprises comme les ressources d'allocation et d'autorité que les auteurs mobilisent dans leur action, et qui vont subsequemment permettre de solliciter des ressources et des informations spécifiques.



![](http://opendatatales.com/wp-content/uploads/2020/07/Figures-graphiques-4.png)
##### Figure : pattern de coordination de l'environnement de conception des usages.

- [ ] réutiliser les carnets sur l'explication de Datafruit pour renseigner ces scenario d'usage. 

Enfin, nous décrirons les fonction du design, c'est à dire "les choses que l'objet designé doit faire pour être une réussite" (Dym et Little, 2004, p.79). Pour cela nous nous sommes basés sur les principes de design construit dans la partie précédente, qui nous a permis d'établir une liste de fonctions, avant de faire des liens avec le design du système et les pattern de coordination. _In fine_, ces fonctions sont peuvent être perçues comme une traduction pratique et concrètes de ces deux éléments.  

