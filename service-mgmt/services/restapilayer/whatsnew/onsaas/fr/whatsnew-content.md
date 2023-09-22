### VMware NSX-T Manager 
#### Avis d'obsolescence 
* VMware NSX Data Center for vSphere (NSX-V) en tant que source de données sera obsolète dans les versions ultérieures. 
* Les services suivants seront affectés après la désapprobation :
    * **Ajout d'une source de données :** Vous ne pourrez pas ajouter NSX-V en tant que source de données.  
    * **Collecte de données :** La collecte de données sera arrêtée et désactivée pour les sources de données NSX-V existantes. 
    * **Mesures et flux :** Les mesures et flux associés seront supprimés conformément à la période de rétention. 
* **Action requise :** Migrez vos instances de NSX-V vers VMware NSX-T et ajoutez des instances de VMware NSX-T en tant que sources de données dans VMware Aria Operations for Networks. 

&nbsp;
&nbsp;
### Assurance réseau et vérification
* Organisez automatiquement l'intégralité de votre mappage réseau ou un ensemble de groupes sélectionnés dans le mappage réseau. Lorsque vous réinitialisez la carte, la disposition est automatiquement ajustée pour s'adapter au mieux à l'écran. 
![](data:image/png;base64,#IMAGEBASE64_auto_arrange.png)
* Sélectionnez en masse plusieurs terminaux sur le mappage réseau et créez facilement des groupes. Vous pouvez également sélectionner plusieurs périphériques et les faire glisser ensemble vers un nouvel emplacement dans le mappage réseau. 
* Créez des groupes à l'aide de l'adresse IP, de la plage d'adresses IP, du sous-réseau et de la recherche personnalisée. Les sources de données récemment ajoutées correspondant aux critères de recherche sont automatiquement incluses dans les groupes appropriés. 
![](data:image/png;base64,#IMAGEBASE64_create_group.png)
* Obtenez des alertes générées par le système si des intentions précédemment définies ne sont pas valides. Vous pouvez également modifier les intentions pour qu'ils correspondent à votre scénario actuel. 
![](data:image/png;base64,#IMAGEBASE64_intent.png)
* Effectuez une recherche de chemin de mappage réseau avec des entités physiques et virtuelles dans lesquelles le nombre total de règles réseau et le nombre total d'entités physiques se trouvent dans leurs limites respectives.  
* Les validations d'intention sont désormais indépendantes du mappage réseau si les limites décrites précédemment sont atteintes. 
* les hôtes VMware ESXi sont désormais automatiquement regroupés dans le mappage réseau en fonction de leurs clusters VMware vCenter respectifs. 
![](data:image/png;base64,#IMAGEBASE64_esxi.png)
* Créez plusieurs groupes dans mappage réseau à l'aide de l'option d'importation CSV via l'interface de ligne de commande.  
![](data:image/png;base64,#IMAGEBASE64_create_groups_through_cli.png)

&nbsp;
&nbsp;
### Améliorations de la plate-forme 
* VMware Aria Operations for Networks prend en charge TLS version 1.3. 
* La coexistence de cpu universel et d'abonnement universel par cœur est désormais prise en charge. Vous pouvez acheter un abonnement universel par cœur pour l'extension alors que votre abonnement CPU universal est toujours actif. L'utilisation s'affiche en termes de cœurs.   
* Vous pouvez désormais configurer des noms d'hôte pour la plate-forme et les collecteurs à l'aide de l'interface de ligne de commande. Ces noms d'hôte s'affichent sur la page Infrastructure et support, les résultats de la recherche, les alertes et la page d'entité. 
![](data:image/png;base64,#IMAGEBASE64_hostnames.png)
* Le corps d'interruption SNMP dans les alertes comporte des champs supplémentaires d'entité et de gestionnaire du problème pour améliorer le temps moyen de réparation (MTTR). 

&nbsp;
&nbsp;
###  
* Ajoutez des périphériques physiques configurés avec des algorithmes de chiffrement plus forts pour les connexions SSH en tant que sources de données gérées. Pour plus d'informations sur les algorithmes de chiffrement pris en charge, reportez-vous à [Chiffrements et chiffrements](https://docs.vmware.com/en/VMware-Aria-Operations-for-Networks/SaaS/Using-Operations-for-Networks/GUID-02B7DC96-66A6-4CDF-9E3E-E25D4C0A8DEC.html)
* Vous pouvez désormais mettre à jour en bloc les informations d'identification SNMP pour des sources de données tierces. 
![](data:image/png;base64,#IMAGEBASE64_snmp.png)
* Vous pouvez désormais exporter les terminaux découverts sous la forme d'un fichier CSV. 
![](data:image/png;base64,#IMAGEBASE64_export_csv.png)
* Vous pouvez désormais importer des terminaux à partir d'un fichier CSV pour les ajouter en tant que sources de données. 
![](data:image/png;base64,#IMAGEBASE64_upload_csv.png)

&nbsp;
&nbsp;
### Découverte d'applications basée sur les flux 
* Vous pouvez désormais télécharger un fichier CSV qui est utilisé par la détection d'applications basée sur les flux (FBAD) pour améliorer la détection des applications. 
    * Utilisez l'exportation CSV à partir d'une base de données de gestion de contenu (CMDB) existante et importez ce fichier CSV pour ajouter des définitions d'applications préexistantes et accélérer le processus de détection d'applications. 
    * Lorsque vous importez un fichier CSV pour découvrir des applications, les noms d'application du fichier CSV sont utilisés pour nommer les applications et les niveaux. 
    * Avant d'enregistrer l'application, vous pouvez modifier ses membres, ses niveaux et son nom. 
    * Les applications créées à l'aide du téléchargement CSV sont surveillées pour les mises à jour et sont affichées sur le tableau de bord des applications pour approbation. 
![](data:image/png;base64,#IMAGEBASE64_upload_csv_fbad.png)
* La découverte d'applications basée sur les flux prend désormais en compte les plages de ports dynamiques lors du regroupement de machines virtuelles dans un niveau.  

&nbsp;
&nbsp;
### Tableaux de bord personnalisés
* Nouveaux widgets disponibles dans la bibliothèque de widgets, tels que les principaux locuteurs, les analyses de flux, les widgets d'application, etc.
* L'utilisateur peut désormais modifier les noms du titre du widget.