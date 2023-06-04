SAE

*Ce document est une structure de base, classique pour rédiger un cahier des charges. Elle est un peu différente de celle vue en TD. Elle n’est pas tout à fait standard non plus en couvrant davantage d’éléments qu’un cahier des charges normal (en particulier le Gantt est fait plus tard normalement, à part ses jalons) Tout ce qui est en italique doit être remplacé. Chaque section doit contenir au moins un paragraphe. Certaines choses sont à imaginer, en se documentant un minimum pour être réaliste.*

![Logo IUT](Aspose.Words.f4dad7c5-82ca-448c-8ff8-8a08a543f2aa.001.png)
# <a name="_f89v6d218qtn"></a>**Cahier des charges fonctionnel - *CAS\_D\_ETUDE***
## <a name="_g0p5anin76na"></a>**Entête**
- Groupe de TD : 1
- Date de démarrage : 10/05/2023
- Version : *Il s'agit d'un numéro de version logique en visant d'arriver à la version 1.0 le jour du rendu (git gère une autre numérotation pour le versionnage*
- Destinataire : *votre chargé de TD*

|**Nom**|**Prénom**|**mail**|
| - | - | - |
|*Bernier*|*Justine*|*justine.bernier1@etu.univ-nantes.fr*|
|*Bruneau rialland*|*Baptiste*|*baptiste.bruneau-rialland@etu.univ-nantes.fr*|
|*Pasquet*|*Clément*|*clement.pasquet@etu.univ-nantes.fr*|
|*Malki*|*Basma*|*basma.malki@etu.univ-nantes.fr*|
## <a name="_ri7lhf8fhbvn"></a>**1. Présentation générale du problème**
### <a name="_upqqsvahyslt"></a>**1.1 Projet**
Le projet est une application mobile, qui permet de donner des informations pour les jeunes personnes asthmatiques entre 12 à 18 ans, et d’aider à prévoir les crises. L'application doit permettre d'apporter un soutien moral aux personnes afin qu’elles puissent mieux gérer les crises. Le projet fait de l’éducation thérapeutique, fournissant des conseils et valorisant différentes informations, également, le projet a pour but de fournir les informations nécessaires aux différents praticiens (médecin généraliste, allergologue, pneumologue, urgentiste …) et d’aider les responsables légaux dans la surveillance de la santé du jeune utilisateur.
#### <a name="_otusm8km61fe"></a>**1.1.1 Finalités**
Avoir une application accessible pour les jeunes qui permet de gérer son asthme. Grâce aux mesures relevées par des capteurs et aux partages de ces informations à l'utilisateur, permettre le suivi de sa santé mais aussi la prédiction d’une potentielle crise d’asthme imminente. Lorsqu’il y a détection d’une future crise d’asthme, l'utilisateur est mis au courant via l’application. De plus, l’application aura une valeur éducative, en informant l’utilisateur sur des études concernant l’asthme ou des sujets voisins avec l'appui d’un comité scientifique afin qu’il puisse mieux appréhender sa maladie. Les informations collectées liées à l'asthme de l’utilisateur seront accessibles pour les professionnels de santé concernés afin d’assurer le suivi de sa santé.

**1.1.2 Espérance de retour sur investissement**

Le financement de l’application et du matériel mis en œuvre sera principalement obtenu par un abonnement qui permet d'utiliser l’application et le matériel.
### <a name="_8dgasr9y2m1g"></a>**1.2 Contexte**
Les études récentes ont démontré que les adolescents souffrant d'asthme ont tendance à ne pas suivre leur traitement, et la majorité des personnes asthmatiques qui se retrouvent aux urgences sont des adolescents. Pour sensibiliser ces jeunes personnes à correctement prendre leur traitement, le moyen le plus efficace est d’utiliser le téléphone qui est un outil dont l’utilisation est très répandu chez les jeunes, et ce pendant une grande partie de leur journée. Pour éviter qu’ils ne renient l'application, elle doit susciter leur intérêt mais ne doit pas être trop invasive.
#### <a name="_px88knfs6jk7"></a>**1.2.1 Situation du projet par rapport aux autres projets de l’entreprise**
L’entreprise a été créée spécifiquement pour le projet, il n’y a donc pas d'autres projets pour l’entreprise.
#### <a name="_bx63scbd2dan"></a>**1.2.2 Études déjà effectuées**
De nombreuses études ont déjà été effectuées concernant l’asthme et plus généralement les capacités respiratoires, et il en est ressorti que les plus touchés par l’asthme sont les mineurs, avec **environ 80% des hospitalisations dues à l’asthme pour les moins de dix-huit ans. ( [Asthme – Santé publique France](https://www.santepubliquefrance.fr/maladies-et-traumatismes/maladies-et-infections-respiratoires/asthme/donnees/#:~:text=La%20pr%C3%A9valence%20de%20l'asthme%20en%20France&text=Quelle%20que%20soit%20la%20vague,16%20%25%20selon%20le%20niveau%20scolaire.&text=a%20Traitement%20pour%20crise%20de,dans%20les%2012%20derniers%20mois) )**

C’est pour cela qu’**il est très important de contrôler l’environnement**. Je cite une étude de l’Agence Nationale d’Accréditation et d’évaluation santé

( [Éducation thérapeutique du patient asthmatique – Adulte et adolescent](https://www.has-sante.fr/upload/docs/application/pdf/education_adulte_asthmatique_-_recommandations.pdf), page 8 ) :

[ … ] *l’éducation thérapeutique doit amener le patient à acquérir les compétences suivantes :*

*- agir sur la présence de facteurs asthmogènes dans son environnement domestique et sa vie sociale et professionnelle*
\*


*- adapter ses activités quotidiennes et de loisirs en fonction de la pollution*

*atmosphérique*

*- agir sur son environnement* [ … ]


De même, je cite : **“*La mise en cohérence des informations est nécessaire à la continuité des soins*”** & **“*Il est recommandé que le patient puisse bénéficier d’une synthèse des données le concernant*”** ( page 11 de l’étude ).

Recommandations qui seront prises en compte lors du développement de l’application.

De même, une majorité des asmathiques n’est pas soumise à de potentielles restrictions d’activitées sportives (cependant, ce n’est pas le cas des Asthmes dit d’Effort), c’est même l’inverse, d’après une étude de la Société Française des Médecines d’Urgence ([Le cœur de l'athlète](https://www.sfmu.org/upload/70_formation/02_eformation/02_congres/Urgences/urgences2013/donnees/pdf/056_Carre.pdf)) :

“*La pratique sportive régulière et modérée est bénéfique pour le système cardiovasculaire.*”, ainsi, notre application contiendra des informations environnementales permettant à l’usager de s’adonner à des activités physiques.

#### <a name="_azsokf29yk9z"></a>**1.2.3 Études menées sur des sujets voisins**
Nous nous basons sur différentes études, comme celle la de l’University of Western Australia ([What is pollen?](https://www.uwa.edu.au/study/-/media/Faculties/Science/Docs/What-is-pollen.pdf)) expliquant le principe du pollen, ou celle de la Société Française de Médecine d’Urgence ([Le cœur de l'athlète](https://www.sfmu.org/upload/70_formation/02_eformation/02_congres/Urgences/urgences2013/donnees/pdf/056_Carre.pdf)) détaillant les différents mécanismes du cœur, et ce que cela signifie.

Et finalement, nous pouvons nous baser sur cette étude ([Mesure sans contact de l'activité cardiaque par analyse du flux vidéo issu d'une caméra numérique](https://theses.hal.science/tel-01751131/document)) qui donne des indices sur ce que pourrait être le futur des mesures - spécialement de l’activité cardiaque - en démontrant que mesurer une activité cardiaque grâce à une caméra thermique est possible.

Il existe aussi différents sites comme Geod’Air ( [Geod'air](https://www.geodair.fr) ) qui permettent d’avoir différentes informations sur l’air en France, ces données sont utiles pour tester les capteurs de qualité de l’air et peuvent servir pour la carte environnementale qui sera dans l’application.

#### <a name="_5q1pf94pgrsb"></a>**1.2.4 Suites prévues**
Il y aura la possibilité de mettre en place dans les communes de petits appareils d’observation de l'environnement. Ils auront pour objectif de prendre des mesures environnementales comme des relevés d'air, de pollen et d’indice de pollution. Ils devront évaluer les changements, les sauvegarder, et faire des corrélations pour mettre en place une carte qui pourra potentiellement prédire les futurs changements d’environnement et donc prédire les périodes de risque potentiel pour les asmathiques selon les zones.

De plus, il y aura à mettre en œuvre une valorisation des données anonymisées de l’utilisateur.

Aussi, il est prévu une avancée technologique dans le projet par le relevé de données de santé via traitement d’images ou de vidéos qui n’est pas invasif pour l’utilisateur.
#### <a name="_vq3nhn90ukx7"></a>**1.2.5 Nature des prestations demandées**

*Développement de l’application*

La conception et le développement d'une application agréable pour les utilisateurs, qui soit compatible avec toutes les plateformes. La conception de l’application devra prendre en compte une interface utilisateur conviviale et intuitive, essentiellement pour faciliter l'utilisation de l'application par les jeunes asthmatiques. Elle devra être attrayante visuellement, facile à naviguer et offrir des instructions claires sur la manière d'effectuer les mesures et d'interpréter les résultats.

*Connection aux appareils de mesure*

L'application devra être capable de se connecter aux appareils de mesures permettant d’évaluer les paramètres respiratoires, tels que le débit expiratoire de pointe (DEP) ou le volume expiratoire maximal seconde (VEMS).

*Collection et stockage sécurisée des données*

L'application doit être capable de collecter, stocker et gérer les données de mesure de chaque utilisateur de manière sécurisée. Les données seront stockées en local sur le téléphone et les données médicales, les profils utilisateur et les historiques de mesures seront envoyés au service numérique de santé tout en permettant à l'utilisateur de décider à qui il partage ses informations.

*Analyse des données*

L'application devra être en mesure d'analyser les données recueillies et d'identifier les tendances, les schémas ou les déclencheurs potentiels de crises d'asthme. Elle pourra également fournir des recommandations personnalisées pour aider les utilisateurs à prévenir les crises, comme des rappels de prise de médicaments ou des conseils sur l'environnement.

*Notifications et alertes*

L'application pourra envoyer des notifications et des alertes aux utilisateurs pour leur rappeler de prendre leurs médicaments, effectuer des mesures régulières ou les informer des niveaux de risque élevés d'une crise imminente.
#### <a name="_kf1udhtwcmrx"></a>**1.2.6 Parties concernées par le déroulement du projet et ses résultats (demandeurs, utilisateurs)**
L’utilisateur mais aussi les praticiens de santé, comme le pneumologue, l’urgentiste, l’allergologue, et les responsables légaux sont concernés par le déroulement du projet.

Les responsables légaux, souvent les parents, ont besoin de consulter et de garder un œil sur les informations médicales de leurs enfants.

Les praticiens de santé (allergologue, urgentiste, généraliste, pneumologue) auront accès aux informations nécessaires à leur pratique médicale, mais pourront aussi prescrire le dispositif médical qui est le produit final de ce projet.

Finalement, l’entreprise est bien sûr aussi concernée par le projet, que ce soit pour la conception, la mise à jour ou le maintien du produit.
#### <a name="_8qhpeimsgnxj"></a>**1.2.7 Caractère confidentiel s'il y a lieu**
Pendant le développement de l’application, l’entreprise va échanger des informations concernant le projet avec les parties concernées et les prestataires.

Ainsi, il sera nécessaire que les parties concernées et les prestataires signent un accord de confidentialité.
### <a name="_811bszn3kohs"></a>**1.3 Énoncé du besoin**
Les besoins diffèrents en fonction des partis. Ainsi, le but principal est d’avertir l’utilisateur,  en cas de crise imminente.

L’application répondra également au besoin de l’utilisateur d’avoir des informations sur son environnement, pour qu’il puisse par lui-même éviter les zones à forte concentration de pollens par exemple.

De même, l’application cherche à informer son utilisateur de manière pédagogique, pour permettre une meilleure compréhension de l’asthme.

Pour les parents, le but est de surveiller leur enfant pour limiter l’impact de potentielles crises, et limiter les risques, mais aussi à terme, de rendre l’enfant plus autonome.

Pour les praticiens, le but est surtout d’accéder aux informations à distance pour permettre un meilleur suivi du patient, permettant de prévenir et anticiper plus facilement les différentes problématiques et difficultés que pourrait rencontrer un patient.

*(finalité du produit pour le futur utilisateur tel que prévu par le demandeur)*
### <a name="_ya5atj9fwpv8"></a>**1.4 Environnement du produit recherché**
#### <a name="_b9ckvblii97f"></a>**1.4.1 Listes exhaustives des éléments *(personnes, équipements, matières…)* et contraintes *(e.g. environnement)***
#### <a name="_o3kru4fqvebx"></a>Besoins > prédire quand une crise va arriver et contrôler l’asthme

<table><tr><th valign="top">Éléments</th><th valign="top">Contraintes</th></tr>
<tr><td rowspan="5" valign="top">Patch</td><td valign="top">Résistance à l’eau</td></tr>
<tr><td valign="top">Résistance aux chocs</td></tr>
<tr><td valign="top">Hypoallergénique (diminue les risques d’allergies)</td></tr>
<tr><td valign="top">Longue Autonomie</td></tr>
<tr><td valign="top">Colle durable</td></tr>
<tr><td valign="top">Transfert de données</td><td valign="top">Connexion & transfert sécurisé de données</td></tr>
<tr><td rowspan="5" valign="top">Stockage de données</td><td valign="top">Stockage local sécuritaire et confidentiel</td></tr>
<tr><td valign="top">Principe de finalité (RGPD) : Choix des données précises, légales et légitimes.</td></tr>
<tr><td valign="top">Principe de proportionnalité et de pertinence ( RGPD ) : Informations enregistrées pertinentes et strictement nécessaires.</td></tr>
<tr><td valign="top">Principe de durée de conservation limitée (RGPD) : la durée de conservation des informations sur l’appareil doit être proportionnelle à leur importance.</td></tr>
<tr><td valign="top">Principe de sécurité et de confidentialité (RGPD)  : Le responsable du fichier doit garantir l’accès aux fichiers en sécurité et en confidentialité.</td></tr>
<tr><td rowspan="3" valign="top">Téléphone</td><td valign="top">Bluetooth existant</td></tr>
<tr><td valign="top">Application installé & patch connecté</td></tr>
<tr><td valign="top">Application mise à jour</td></tr>
<tr><td rowspan="3" valign="top">Projet de postes d’observation environnemental</td><td valign="top">Autorisation de poser ces postes dans chaques communes</td></tr>
<tr><td valign="top">Sauvegarde de l'entièreté des données et gestion de backup</td></tr>
<tr><td valign="top">Intégrité du système lors du piratage des boite, et protection serveur global</td></tr>
<tr><td valign="top">Capteurs</td><td valign="top">Savoir si l’information relevée est bonne</td></tr>
<tr><td valign="top">Capteurs environnementaux</td><td valign="top">N’envoyer que les informations pertinentes sur l'environnement extérieur (par exemple : les données relevées ayant des résultats anormaux, un taux élevé de …)</td></tr>
</table>

Sources: https://www.cnil.fr/fr/cnil-direct/question/quels-sont-les-grands-principes-des-regles-de-protection-des-donnees
#### <a name="_yc6qgbi8tsdo"></a>**1.4.2 Caractéristiques pour chaque élément de l’environnement**
#### <a name="_f8zrbv5je6g4"></a>Caractéristiques des patchs :
- Résistance à l’eau : Un des deux patchs étant prévus pour être porté à même la peau, il est important qu’il soit résistant à l’eau, que ce soit pour des raisons pratiques (que les patchs puissent être portés pendant les douches, bain, etc… ) ou à cause de l’environnement (pluie).
- Résistance aux chocs : pour les mêmes raisons, le patch doit résister au quotidien de n’importe qui.
- Hypoallergénique : le patch ne peut pas provoquer d’infections ou d’allergies sur la partie du corps sur lequel il est posé.
- Longue Autonomie : Le patch doit être capable d’envoyer des informations au téléphone sur une large durée, sans avoir besoin de recharger ou de changer le patch régulièrement, ce qui poserait plus de problèmes.
- Colle durable : Pour les mêmes raisons que précédemment, il est important d’avoir une colle solide, résistante entre autres à l’eau, ce qui diminue le besoin de la remplacer afin que le port du patch ne soit en aucun cas pénalisant ou trop contraignant.
- Batterie durable, qui ne se déchargera pas toute seule sur une grosse période de temps.
- Émetteur : un émetteur onde fonctionnant avec le bluetooth , il doit être performant et très optimisé pour limiter le déchargement de la batterie.
- Récepteur : va de paire avec l'émetteur bluetooth, le mieux est que ce composant soit le même que celui qui gèrent emission bluetooth.



Collecte des données :

- Connexion & transfert sécurisé de données : Le smartphone et les patchs doivent communiquer de manière sécurisée et confidentielle, empêchant d’autres acteurs d’y avoir accès.
- Stockage de données : Le stockage doit être local, autrement dit tout doit être stocké sur le smartphone de l’utilisateur, et cela en toute sécurité et confidentialité.
- Principe de finalité : Une des caractéristiques principales du RGPD selon la CNIL est que les données doivent être précises, légales et légitimes.
- Principe de proportionnalité et de pertinence : Une des caractéristiques principales du RGPD, les informations enregistrées doivent être pertinentes et strictement nécessaires.
- Principe de durée de conservation : Une des caractéristiques principales du RGPD, la durée de conservation des informations sur l’appareil (le smartphone de l’utilisateur) doit être proportionnelle à leur importance, et les supprimer dans le cas contraire.
- Principe de sécurité et de confidentialité : Une des caractéristiques principales du RGPD, le responsable du fichier doit garantir l’accès aux fichiers en sécurité et en confidentialité.

Téléphone :

- Bluetooth compatible : Le téléphone **doit** disposer du bluetooth.
- Application installée & patch connecté : pour des raisons pratiques, le téléphone doit avoir l’application d’installée et le patch connecté.

## <a name="_4yuplcrsvr5k"></a>**2. Expression fonctionnelle du besoin**
*Le **+** à priori chaque cas d’utilisation correspond à une fonction. Le diagramme de cas d’utilisations inclut la description détaillée de chaques cas d’utilisations (cf. cours de CO-C).*

*Chaques fonctions doivent être classées selon différents critères :*

- *coefficient de pondération (de 1 à 5) : selon la valeur, l’importance de la fonction*
- *critère d’appréciation : comment sera apprécié le succès de la réalisation d’une fonction (« doit rendre le résultat correct en moins de x secondes »)*
- *niveau d’un critère d’appréciation (« x de 1 à 3 secondes acceptables »)*
- *niveau de flexibilité (« 90% dans l’intervalle, 10% à 1 seconde au-delà »)* *On peut regrouper les fonctions dans le **tableau fonctionnel** selon ces critères puis détailler chacune des fonctions dans les sous-sections suivantes.*

![](./Aspose.Words.f4dad7c5-82ca-448c-8ff8-8a08a543f2aa.002.png)
![](./Aspose.Words.f4dad7c5-82ca-448c-8ff8-8a08a543f2aa.003.png)

### <a name="_yr4pyd6oo52b"></a>**2.1 Fonctions de service et de contrainte**
#### <a name="_vr8a2ou78h2i"></a>**2.1.1 Fonctions de service principales**
- Mesurer les différents paramètres de santé de l’utilisateur
- Envoyer les données de santé de l’utilisateur au téléphone
- Partager les données de santé du téléphone de l’utilisateur à l’Espace Numérique de Santé
- Alerter l’utilisateur pendant la crise (rassurer l’utilisateur)
- Prévenir l’utilisateur d’une future crise
- Eduquer l’utilisateur en vulgarisant l’asthme et les sujets connexes (Informations faites vérifiées par le comité médical)

##### <a name="_x7erz4i40f8f"></a>**2.1.1.1 Description et détail**
Mesurer les différents paramètres de santé de l’utilisateur : il faut récupérer  différentes informations physiques provenant du corps du porteur du patch (taux d’oxygène dans le sang, taux de glucose…). L’asthme est provoqué par plusieurs facteurs agissant sur le corps. Selon la personne, l’asthme peut se déclencher via certains paramètres comme la quantité d'oxygène dans le sang, le rythme cardiaque qui détermine la vitesse d'acheminement de l'oxygène, le taux de glucose ou encore la température du corps.  Ainsi il est important de récolter ces données.

Envoyer les données de santé de l’utilisateur au téléphone : Les patchs récoltant les informations, il faut les envoyer au téléphone relié en bluetooth.

Partager les données de santé du téléphone de l’utilisateur à l’Espace Numérique de Santé : Le téléphone envoie les informations récupérées à l’Espace Numérique de Santé du patient.

Alerter l’utilisateur en cas de crise : Si le patch détecte que l’utilisateur est en crise ou va être en crise très prochainement, l’application envoie différents signaux (messages, notifications, alerte(s)…)

Prévenir l’utilisateur : Si le patch permet de remarquer que le patient risque d’être en crise prochainement mais pas de façon imminente, l’application préviendra l’utilisateur, mais avec des signaux moins forts, de manière à le conseiller et le rassurer (pas ou moins d’alarmes…)

Eduquer l’utilisateur : Il faut informer l’utilisateur de différentes informations sur l’environnement (taux de pollen présents et futures, zones à risques…) mais aussi de différentes informations pédagogiques (conseils pour ne pas paniquer, recommandations de précautions, fonctionnement de l’asthme…) plus précis.
##### <a name="_gta0usuf2qd4"></a>**2.1.1.2 Critères d’appréciation et les niveaux qui les caractérisent**
*(Niveaux dont l’obtention est imposée)*

*(Niveaux souhaités mais révisables)*



|Nom|Coef. de Pondération|Critères d’Appréciation|Niv. des crit. d’Appréciation|Niveaux de Flexibilité|
| :- | :- | :- | :- | :- |
|Mesurer les différents paramètres de santé de l’utilisateur|5|Le patch dispose des informations de santé au moins toutes les 5 minutes.|Info. de santés mesurées toutes les 1 à 2 minutes préférables.|Au maximum une quinzaine de secondes.|
|Envoyer les données de santé de l’utilisateur au téléphone|5|` `Les informations sont envoyées au moins toutes les 5 minutes.|Info. de santés envoyées toutes les 1 à 2 minutes préférables.|Au maximum une quinzaine de secondes.|
|Partager les données de santé du téléphone de l’utilisateur à l’Espace Numérique de Santé|4|Les données de santé peuvent être envoyées au maximum toutes les semaines.|Les données de santé doivent être envoyées au mieux tous les jours.|15 minutes, le temps que la synchronisation se fasse.|
|Alerter l’utilisateur en cas de crise|5|Que l’utilisateur soit alerté immédiatement ou en un très court délai, de maximum 30 secondes.|Pour permettre une action immédiate, au maximum une quinzaine de secondes.|~ 3 secondes.|
|Prévenir l’utilisateur|3|Si il n’y a pas d’alerte, alors le rythme d’information peut être, au maximum une dizaine de minutes.|Que l’utilisateur soit informé en 5 minutes des informations sur l'environnement.|~ 1 minute.|
|Education Pédagogique|3|L’utilisateur doit recevoir de nouveaux conseils régulièrement, au minimum tous les 3 jours.|Il serait préférable de recevoir des informations tout les 2 jours|~ 2 heures.|

#### <a name="_i33hipma49t1"></a>**2.1.2 Fonctions de service complémentaires**
- L'application prévient quand le patch est bientôt déchargé
- L’utilisateur a la possibilité de renseigner la carte avec les mesures d'environnement avec des appareils de mesure.

*(qui améliorent, facilitent ou complètent le service rendu)*
##### <a name="_q12jknotbhmi"></a>**2.1.2.1 Description et détail**

L'application prévient quand le patch est bientôt déchargé : L’application doit prévenir au moins 1 semaine à l’avance pour que le patch puisse être délivré à temps.

Niveau souhaité : l’application doit prévenir au mieux 2 semaines à l’avance pour pouvoir changer au plus vite son patch. L’état de chargement doit être communiqué en pourcentage et non en temps afin qu’il soit plus parlant pour l’utilisateur.

L’utilisateur a la possibilité de renseigner la carte avec les mesures d'environnement avec des appareils de mesure : comme l’application contient une carte, on pourra agrémenter cette carte avec nos propres informations.

##### <a name="_kslh1u3niuew"></a>**2.1.2.2 Critères d’appréciation et les niveaux qui les caractérisent**




|Nom|Coef. de Pondération|Critères d’Appréciation|Niv. des crit. d’Appréciation|Niveaux de Flexibilité|
| :- | :- | :- | :- | :- |
|L'application prévient quand le patch est bientôt déchargé|4|L’application devra prévenir quand le patch n’aura plus que 10 % de batterie..|Au mieux, l’application prévient quand la batterie n’a plus que 15%.|A environ 1% près.|
|L’application prévient lorsqu’un capteur produit des données aberrantes|3|Données incohérentes, valeurs très hautes ou très faibles|Données incohérentes, valeurs très hautes ou très faibles|` `Environ 5% des données venant d’être récoltées sur une période de plus ou moins 45 secondes sont  incohérentes.|

*(Niveaux dont l’obtention est imposée)*

*(Niveaux souhaités mais révisables)*
#### <a name="_27r1jnjd0hx8"></a>**2.1.3 Contraintes**
*(limitations à la liberté du concepteur-réalisateur)*

- Les différentes liaisons (entre les patchs et le téléphone, et entre le téléphone et l’Espace Numérique de Santé) doivent être sécurisées.