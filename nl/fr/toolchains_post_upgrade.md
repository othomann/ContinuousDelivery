---

copyright:
  years: 2015, 2018
lastupdated: "2018-1-12"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Initiation aux chaînes d'outils après la mise à niveau de votre projet {{site.data.keyword.jazzhub_short}}
{: #toolchains_post_upgrade}

Les projets {{site.data.keyword.jazzhub}} sur hub.jazz.net ont été convertis en chaînes d'outils dans le service {{site.data.keyword.Bluemix_notm}} {{site.data.keyword.contdelivery_short}}. 

{{site.data.keyword.jazzhub_short}} sur hub.jazz.net est retiré. 

Pour vos projets DevOps, utilisez le [service {{site.data.keyword.contdelivery_short}} ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://console.bluemix.net/devops){:new_window}. Si vous ne maîtrisez pas encore {{site.data.keyword.Bluemix_notm}}, prenez soin de lire la [présentation d'{{site.data.keyword.Bluemix_notm}}](/docs/overview/whatisbluemix.html#bluemixoverview).

{: shortdesc}

## Recherche de la chaîne d'outils qui a été créée à partir de votre projet
{: #find_toolchain}

Vérifiez que la mise à niveau est terminée en vous rendant sur la [page Chaînes d'outils![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://console.bluemix.net/devops/toolchains){: new_window} et en vérifiant que des chaînes d'outils  portant le même nom que vos projets hub.jazz.net sont affichées. Si vos projets ont été automatiquement mis à niveau, conservez les restrictions suivantes à l'esprit :
   - Si une autre chaîne d'outils avait déjà utilisé le nom de votre projet avant que celui-ci ne soit mis à niveau, la nouvelle chaîne d'outils qui a été créée pour votre projet peut ne pas porter le même nom que votre projet. 
   - Si vous ne voyez aucune chaîne d'outils pour votre projet, passez dans une autre organisation dont vous êtes membre et vérifiez les chaînes d'outils qu'elle contient.
   - Si la chaîne d'outils de l'un de vos projets reste introuvable, il se peut que sa mise à niveau soit toujours en cours. Si vous avez besoin d'accéder immédiatement à cette chaîne d'outils, contactez le [support ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://developer.ibm.com/answers/questions/ask/?smartspace=devops-services){:new_window}.

## Présentation des chaînes d'outils
{: #compare_toolchains}

Si vous possédiez un ou plusieurs projets sur hub.jazz.net, ils ont été automatiquement convertis en chaînes d'outils dans le service {{site.data.keyword.contdelivery_short}}, à moins que la mise à niveau ait échoué. Les mises à niveau peuvent échouer en raison de comptes IBM Cloud ou organisation non valides. Ces propriétaires de comptes et d'organisations ont été informés par courrier électronique des défaillances et des actions spécifiques requises de leur part pour y remédier. Si vous ne voyez pas la chaîne d'outils relative à votre projet et que vous avez besoin d'accéder immédiatement à cette chaîne d'outils, contactez le [support ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://developer.ibm.com/answers/questions/ask/?smartspace=devops-services){:new_window}. 

Les chaînes d'outils sont semblables à des projets, à quelques différences importantes près :

- Les projets ne peuvent avoir qu'un seul référentiel et qu'un seul pipeline. Les chaînes d'outils peuvent avoir autant de référentiels et de pipelines que nécessaire.
- Les chaînes d'outils peuvent inclure des outils qui ne sont pas disponibles dans des projets, tels que Slack, Sauce Labs, PagerDuty et {{site.data.keyword.DRA_full}}.

 **Remarque** : {{site.data.keyword.DRA_short}} est uniquement disponible dans la région sud des Etats-Unis.
 
- Dans les projets, l'appartenance est gérée au niveau du projet. L'accès aux chaînes d'outils est géré par l'organisation {{site.data.keyword.Bluemix_notm}} et par la chaîne d'outils. Pour gérer une chaîne d'outils, vous devez être membre de l'organisation qui la contient. Le propriétaire de la chaîne d'outils peut davantage contrôler qui peut accéder à la chaîne d'outils et ce que cette personne est autorisée à faire. Pour plus d'informations, voir l'étape 2 dans la rubrique [Initiation à votre chaîne d'outils](#upgrade_next_steps).
- Selon le type de référentiel que vous avez utilisé dans votre projet sur hub.jazz.net, votre chaîne d'outils peut contenir un référentiel GitHub.com ou un référentiel {{site.data.keyword.gitrepos}}.

Pour en savoir plus sur les chaînes d'outils, consultez [YouTube ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://youtu.be/2SIPE1e7NJ4){: new_window} ou [Initiation à {{site.data.keyword.contdelivery_short}}](/docs/services/ContinuousDelivery/index.html).

## Initiation à votre chaîne d'outils
{: #upgrade_next_steps}

1. Accordez l'accès à la chaîne d'outils aux membres de votre équipe.
    - Chaque membre d'équipe doit disposer d'un compte {{site.data.keyword.Bluemix_notm}} valide. Les membres de l'équipe qui ne possèdent pas de comptes doivent [s'enregistrer![Icône de lien externe](../../icons/launch-glyph.svg "External link icon")](https://console.ng.bluemix.net/registration){:new_window}.
    - Accordez aux membres de l'organisation un accès à la chaîne d'outils depuis la page Gérer de la chaîne d'outils. Des membres de projet existants sont ajoutés en tant que membres de la chaîne d'outils dans le cadre du processus de mise à niveau. Pour en savoir plus sur le contrôle d'accès aux chaînes d'outils, voir [Gestion des accès ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](/docs/services/ContinuousDelivery/toolchains_using.html#managing_access){:new_window}.
    - Si un utilisateur n'est pas membre de l'organisation à laquelle appartient la chaîne d'outils, ajoutez-le à l'organisation depuis la page Gérer les organisations.
    - Si votre chaîne d'outils utilise {{site.data.keyword.gitrepos}}, tous les membres du projet JazzHub dotés d'un ID {{site.data.keyword.Bluemix_notm}} valide sont ajoutés au référentiel {{site.data.keyword.gitrepos}} avec les mêmes privilèges que ceux qu'ils avaient dans le projet JazzHub. Si votre projet JazzHub comprend des membres qui ne disposent pas d'un ID {{site.data.keyword.Bluemix_notm}} valides, ceux-ci peuvent s'inscrire pour en obtenir un. Une fois qu'ils se sont inscrits, vous pouvez les ajouter au référentiel.
      Pour obtenir des informations complémentaires sur la gestion des organisations, voir [Gestion des organisations et des espaces ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](/docs/admin/orgs_spaces.html#orgsspacesusers){:new_window}.

2. Si vous utilisez {{site.data.keyword.gitrepos}}, authentifiez-vous à l'aide d'un jeton d'accès personnel ou d'une clé SSH. Pour en savoir plus sur les clés SSH, voir [Création d'un jeton d'accès personnel ou d'une clé SSH pour l'authentification](/docs/services/ContinuousDelivery/git_working.html#git_authentication). Pour s'authentifier depuis un client Git externe via https, procédez comme suit :
    1. Accédez à la page [Jetons d'accès ![Icône de lien externe](../../icons/launch-glyph.svg "External link icon")](https://git.ng.bluemix.net/profile/personal_access_tokens){:new_window} de vos paramètres utilisateurs {{site.data.keyword.gitrepos}}.
    2. Créez un jeton d'accès personnel utilisant **api** comme portée.
    3. Accédez à la page [Compte ![Icône de lien externe](../../icons/launch-glyph.svg "External link icon")](https://git.ng.bluemix.net/profile/account){:new_window} et recherchez votre nom d'utilisateur pour {{site.data.keyword.gitrepos}}. Votre nom d'utilisateur est répertorié dans la section "Changer le nom d'utilisateur" et apparaît dans la première partie de l'URL des référentiels personnels que vous créez.
    4. Pour vous authentifier auprès de {{site.data.keyword.gitrepos}} depuis un client Git externe via HTTPS, utilisez votre nom d'utilisateur et votre jeton d'accès personnel.
    5. Si vous souhaitez réutiliser le référentiel local de votre référentiel JazzHub Git, faites pointer le référentiel vers le nouveau référentiel dans {{site.data.keyword.gitrepos}}. Depuis un interpréteur de commande shell dans un terminal, accédez au répertoire dans lequel le référentiel JazzHub Git est cloné. Entrez la commande `git remote set-url` : `git remote set-url origin https://git.ng.bluemix.net/<userid>/<name-of-new-repo>`

        **Astuce :** pour vérifier quelles URL distantes sont définies sur quels noms distants, utilisez la commande `git remote -v`. Le nom distant
par défaut est `origin`. Si vous disposez d'une configuration plus avancée, le format de la commande est le suivant : `git remote set-url <remote-name-that-uses-jazzhub-repo> https://git.ng.bluemix.net/<userid>/<name-of-new-repo>`

3. Facultatif : pour explorer la maturité du développement de votre projet, les pratiques de votre équipe et la qualité de votre codebase, ajoutez IBM Cloud
{{site.data.keyword.DRA_short}} à votre chaîne d'outils. {{site.data.keyword.DRA_short}} applique les analyses de déploiement, le développeur et l'équipe aux projets DevOps. Pour
plus d'informations, voir [Initiation à {{site.data.keyword.DRA_short}}](/docs/services/DevOpsInsights/index.html).

  **Remarque** : {{site.data.keyword.DRA_short}} est uniquement disponible dans la région sud des Etats-Unis.


## Traitement des incidents
{: #upgrade_troubleshoot}

Si des problèmes liés à la mise à niveau de votre projet se produisent, publiez une question sur le [forum de support ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://developer.ibm.com/answers/questions/ask/?smartspace=devops-services){:new_window}. Dans l'article que vous publiez sur le forum, incluez les URL à votre projet {{site.data.keyword.jazzhub_short}} et votre chaîne d'outils {{site.data.keyword.contdelivery_short}} et signalez votre
publication avec l'étiquette `devops-services`.


## Foire aux questions
{: #upgrade_faq}

### Mon projet JazzHub a été associé à la région Royaume-Uni, mais ma chaîne d'outils se trouve dans la région Sud des Etats-Unis. Comment cela fonctionne ?
{: #faq_region}

Les projets sur hub.jazz.net et les chaînes d'outils sont hébergés dans la région Sud des Etats-Unis. Si votre projet a été configuré pour déployer des applications dans une région différente, comme la région UK, la chaîne d'outils déploiera quand même les applications dans cette région également. Par conséquent, aucune modification n'est réellement apportée quant à l'emplacement d'hébergement des données. A l'avenir, les chaînes d'outils seront disponibles dans davantage de régions.

### Qu'advient-il de mes éléments de travail et de mes tableaux de bord dans Track &amp; Plan après la mise à niveau ?
{: #faq_tp}

Le service {{site.data.keyword.contdelivery_short}} fournit des fonctions de suivi des problèmes grâce à {{site.data.keyword.gitrepos}}, hébergé par IBM et basé sur GitLab Community Edition. {{site.data.keyword.contdelivery_short}} prend également en charge les intégrations dotées d'autres outils de planification et de suivi des problèmes, tels que GitHub Issues et JIRA.

Durant le processus de mise à niveau, vos éléments de travail Track & Plan ont été migrés vers Git Issues. GitHub Issues et {{site.data.keyword.gitrepos}} fournissent des tableaux Kanban et un système de suivi des problèmes pour la planification. Pour en savoir plus sur Issue Boards, qui est la fonction kanban de Git Repos and Issue Tracking, voir [Issue board ![Icône de lien externe](../../icons/launch-glyph.svg "External link icon")](https://git.ng.bluemix.net/help/user/project/issue_board.md){: new_window}.

Si vous avez besoin de la même fonctionnalité que le composant JazzHub Track &amp; Plan désormais obsolète, un nouveau service IBM Track and Plan on Cloud est disponible et peut être acheté dans certains pays sur une base mensuelle par utilisateur. Ce service de cloud vous permet de bénéficier de fonctions complètes, équivalentes aux licences contributeur Rational Team Concert&trade;, avec un abonnement de cloud à service exclusif.

Ce nouveau service IBM Track and Plan on Cloud propose une fonctionnalité beaucoup plus riche que la fonction obsolète JazzHub Track &amp; Plan, en prenant en charge la personnalisation des processus, les hiérarchies de projet, SAFe&reg; et de nombreuses autres méthodes hybrides et agiles, tout en garantissant l'évolutivité qui permet une croissance au-delà d'un simple projet. Il repose sur la version la plus récente de Rational Team Concert 6.0.3 et sera au niveau de la version 6.0.4 dans les 60 prochains jours, alors que JazzHub Track &amp; Plan était basé sur Rational Team Concert 5.x. Il est possible de migrer les données vers IBM Track and Plan on Cloud grâce à des services supplémentaires. Pour plus d'informations, vous pouvez contacter [Tom Hollowell ![Icône de lien externe](../../icons/launch-glyph.svg "External link icon")](mailto:trhollow@us.ibm.com){:new_window}, Responsable des ventes SaaS des produits connectés.

Pour plus d'informations sur IBM Track and Plan on Cloud, ou pour effectuer un achat en ligne, visitez le site Web [IBM Marketplace ![Icône de lien externe](../../icons/launch-glyph.svg "External link icon")](https://www.ibm.com/us-en/marketplace/cloud-change-management){: new_window}.

[Rational Team Concert on Cloud ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://www.ibm.com/us-en/marketplace/change-and-configuration-management/purchase#product-header-top){: new_window} vous permet de bénéficier en plus des fonctions d'automatisation de la construction et de gestion du code source.

### Qu'advient-il de mon référentiel de code après la mise à niveau ?
{: #faq_repo}

Une fois la mise à niveau effectuée, votre nouveau service Git est comparable à ce que vous aviez auparavant. Si vous utilisiez github.com avec votre projet JazzHub, votre chaîne d'outils est connectée au même référentiel GitHub. Si votre projet JazzHub utilisait le référentiel Git hébergé par IBM, le contenu de ce référentiel est cloné vers un nouveau référentiel dans {{site.data.keyword.gitrepos}}, qui fait partie de {{site.data.keyword.contdelivery_short}} et est hébergé par IBM.

Pour plus d'informations sur la manière dont chaque type de référentiel est traité lors de la mise à niveau, reportez-vous au tableau ci-dessous.

|Référentiel de projet |Type de projet	|Référentiel de chaîne d'outils |
|:----------|:------------------------------|:------------------|
|github.com 		|Privé ou public 		|Le même référentiel github.com avec {{site.data.keyword.Bluemix_notm}} Public.	|
|hub.jazz.net/git		|Privé ou public 		|Un nouveau référentiel privé ou public dans {{site.data.keyword.gitrepos}} avec {{site.data.keyword.Bluemix_notm}} Public.	|
|Jazz SCM		|Privé ou public 		|Un nouveau référentiel privé ou public dans {{site.data.keyword.gitrepos}} avec {{site.data.keyword.Bluemix_notm}} Public.	|
{: caption="Tableau 1. Référentiels de projet mappés à des référentiels de chaîne d'outils" caption-side="top"}


### Qu'advient-il de mes définitions de génération dans mon projet après la mise à niveau ?
{: #faq_build}

Si vous génériez votre code source avec Jazz à la place de Delivery Pipeline, vous devez migrer manuellement vos définitions de génération vers Delivery Pipeline dans votre chaîne d'outils.

Si vous utilisiez Jazz SCM comme référentiel source et Delivery Pipeline pour générer votre code, le code source de Jazz SCM a été automatiquement déplacé vers un référentiel Git. Votre configuration Delivery Pipeline reste la même, mais consomme le code source du référentiel Git au lieu du code source de Jazz SCM.

### J'ai dû créer une organisation pour mon projet qui a été mis à jour vers une chaîne d'outils. Pour cela, j'ai ajouté une carte de crédit à mon compte. Ma carte de crédit sera-t-elle débitée ?
{: #faq_charges}

En tant que [client de type Paiement à la carte ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://www.ibm.com/cloud-computing/bluemix/pricing){: new_window}, si vous utilisez un contexte d'exécution, un service ou un composant au-delà des allocations gratuites répertoriées dans le catalogue {{site.data.keyword.Bluemix_notm}}, vous êtes facturé. Pour avoir une estimation de votre utilisation, reportez-vous à la  [fiche de prix ![Icône de lien externe](../../icons/launch-glyph.svg "External link icon")](https://console.ng.bluemix.net/?direct=classic/&cm_mc_uid=49681106114614956310454&cm_mc_sid_50200000=1495641296&cm_mc_sid_52640000=1494981898#/pricing/cloudOEPaneId=pricing&paneId=pricingSheet){: new_window}. Pour connaître la tarification en vigueur de Continuous Delivery, voir le [catalogue {{site.data.keyword.Bluemix_notm}} ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://console.bluemix.net/catalog/services/continuous-delivery){: new_window}.

Si vous êtes un employé d'IBM, les projets IBM internes peuvent être facturés aux départements, à la place d'une carte de crédit personnelle. Si vous avez besoin d'utiliser des ressources au-delà des allocations gratuites destinées aux employés IBM, créez un ticket de demande de service.

### Ma chaîne d'outils est introuvable ou inaccessible. Que dois-je faire ?
{: #faq_find}

Les chaînes d'outils sont hébergées dans les organisations {{site.data.keyword.Bluemix_notm}}. Le processus de mise à niveau ajoute tous les membres du projet JazzHub à la chaîne d'outils. Cela dit, si ces utilisateurs ne sont pas ajoutés à l'organisation {{site.data.keyword.Bluemix_notm}} par le propriétaire de cette dernière, ils ne peuvent pas voir la chaîne d'outils. 

Pour accéder à votre chaîne d'outils, accédez à {{site.data.keyword.Bluemix_notm}}, cliquez sur l'icône de menu, puis sur **Services &gt; DevOps**. La page Chaîne d'outils s'affiche. Vérifiez que vous vous trouvez dans la région Sud des Etats-Unis et que vous avez été ajouté à l'organisation qui contient la chaîne d'outils. Si votre chaîne d'outils n'apparaît pas sur la page Chaînes d'outils, consultez [cette entrée de FAQ](#faq_uk).

### Mon projet est associé à la région Royaume-Uni. Après la mise à niveau, des messages d'erreur apparaissent, mes collègues ne peuvent pas accéder à la chaîne d'outils et ma chaîne d'outils n'apparaît pas sur la page Chaînes d'outils de {{site.data.keyword.Bluemix_notm}}. Qu'est-ce qui ne va pas ?
{: #faq_uk}

**Question complète :**

Mon projet JazzHub est associé à la région Royaume-Uni de {{site.data.keyword.Bluemix_notm}} conformément aux paramètres du projet. J'ai vérifié les paramètres de mon projet en accédant à la page de présentation le concernant sur JazzHub, en cliquant sur l'icône **Settings** (qui ressemble à un engrenage) et en cliquant sur **Options &gt; Make this a {{site.data.keyword.Bluemix_notm}} Project: Region**. Après la mise à niveau du projet vers une chaîne d'outils aux Etats-Unis, les problèmes suivants se sont produits :

   1. Lorsque je sélectionne l'organisation américaine, un message indiquant que cette organisation ne comporte pas d'espace dans la région Sud des Etats-Unis s'affiche et je suis invité à créer un espace. Je ne veux rien exécuter aux Etats-Unis.
   
   2. Certains de mes collègues ne peuvent pas accéder à la chaîne d'outils, pourtant ils apparaissaient en tant que membres dans le projet JazzHub initial. S'ils tentent d'ouvrir la chaîne d'outils à partir de la page de présentation de l'application dans la région Etats-Unis en cliquant sur **Afficher la chaîne d'outils**, un message "accès refusé"  s'affiche.
   
   3. La chaîne d'outils répertoriée sur ma page Chaînes d'outils n'apparaît pas sur [https://console.bluemix.net/devops/toolchains?env_id=ibm:yp:us-south ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://console.bluemix.net/devops/toolchains?env_id=ibm:yp:us-south){: new_window}, en revanche, je peux y accéder directement à partir de la page de présentation de l'application dans la région Etats-Unis en cliquant sur **Afficher la chaîne d'outils**. J'obtiens un message d'erreur indiquant que je ne peux pas modifier la chaîne d'outils ou que je possède pas de chaîne d'outils et que je dois en créer une. 

**Réponse :**

Ces problèmes peuvent se produire si vous êtes issu d'une organisation {{site.data.keyword.Bluemix_notm}} non américaine et que vous n'avez pas étendu explicitement votre organisation dans la région Sud des Etats-Unis avant la mise à niveau. Vous pouvez vérifier ceci en ouvrant la page Chaînes d'outils. Vous trouverez la région et l'organisation au début de la page. 

Voici ce qu'il s'est passé : au moment de la mise à niveau, votre organisation non américaine n'existait pas aux Etats-Unis, par conséquent, la mise à niveau a sélectionné une autre organisation pour vous en en recherchant une autre à laquelle il vous est arrivé d'accéder.

Si vous passez dans cette organisation {{site.data.keyword.Bluemix_notm}} américaine, la chaîne d'outils apparaîtra. Si vous ajoutez vos collègues à cette organisation, un accès leur sera accordé. Cette chaîne d'outils peut continuer à être déployée sur votre organisation non américaine. Le seul problème est que ces deux organisations sont distinctes ; la gestion des utilisateurs ne peut pas s'effectuer automatiquement sur les deux.

Si vous souhaitez que votre chaîne d'outils figure dans une organisation américaine correspondant à votre organisation non américaine, procédez comme suit :

   1. Connectez-vous à [https://console.bluemix.net ![Icône de lien externe](../../icons/launch-glyph.svg "Icône de lien externe")](https://console.bluemix.net){: new_window} et sélectionnez la région et l'organisation non américaines dont vous êtes issu.
   
   2. Dans l'en-tête {{site.data.keyword.Bluemix_notm}}, passez dans la région Sud des Etats-Unis. Vous serez invité à créer un espace dans cette région.
   
   3. Créez un espace dans la région Sud des Etats pour étendre votre organisations dans cette région. 
   
   4. Supprimez la chaîne d'outils qui a été créée via le processus de mise à niveau. 
   
      **Remarque :** le référentiel Git n'est pas supprimé automatiquement. Vous souhaiterez peut-être le supprimer manuellement ou le renommer pour le moment. Si vous l'avez déjà modifié, vous pourrez passer à la future chaîne d'outils pour l'utiliser ultérieurement.

   5. Revenez au projet JazzHub. Normalement, il doit être automatiquement réinitialisé pour permettre une autre tentative de mise à niveau. Si tel n'est pas le cas, contactez hub@jazz.net en indiquant l'URL du projet.
   
   6. Redémarrez le processus de mise à niveau en prenant soin de sélectionner l'organisation dans la région Etats-Unis qui correspond au nom de votre organisation dans la région hors des Etats-Unis.
   
   7. Si vous avez conservé ou renommé le référentiel Git issu de votre précédente tentative de mise à niveau de chaîne d'outils (voir l'étape 4), vous pouvez reconfigurer la carte Git dans votre chaîne d'outils pour qu'elle pointe vers l'URL du référentiel Git. Cette modification est automatiquement répercutée dans le pipeline. Pour le vérifier, consultez l'onglet Entrée sur l'étape Génération.
