# Docker

### Cluster de conteneurs et Orchestration

**Faites une recherche avancée sur la clusterisation des conteneurs**

+ Les clusters de conteneurs permettent de répartir les applications sur plusieurs conteneurs et machines hôtes. Si un conteneur ou une machine tombe en panne, le cluster peut rediriger le trafic ou redémarrer les conteneurs sur d'autres machines.
+ Ils facilitent la montée en charge et la réduction de charge des applications en fonction de la demande, ce qui permet d'ajouter ou de supprimer des conteneurs dynamiquement.
+ Ils offrent des mécanismes pour déployer de nouvelles versions d'applications ou effectuer des mises à jour sans temps d'arrêt.
+ Les plus populaires sont Docker Swarm et Kubernetes

**Faites une recherche sur le concept de microservice**

Tout d'abord, un microservice est une architecture logicielle où une application est divisée en un ensemble de services plus petits et indépendants. Chaque service est responsable d'une fonctionnalité spécifique et peut être développé, déployé, et géré de manière indépendante.

Dans le cadre de Docker, celui-ci peut conteneuriser ces services, ainsi, chaque microservice fonctionne de manière cohérente dans différents environnements, que ce soit en développement, en test ou en production.

**Faites une recherche sur les concepts de scalability, availability et Le load Balancing**

**Scalability**

La scalabilité est la capacité d'un système à gérer une charge croissante en ajoutant des ressources, soit de manière horizontale (ajout de plus de serveurs), soit de manière verticale (ajout de plus de puissance de calcul à un serveur existant).

**Availability**

La disponibilité fait référence à la capacité d'un système à rester opérationnel et accessible, même en cas de défaillance de certains de ses composants. Grâce aux clusters de conteneurs comme Kubernetes ou Docker Swarm, il est possible de gérer automatiquement la scalabilité en fonction de la demande. Docker contribue à la haute disponibilité en isolant les applications dans des conteneurs. Cela signifie qu'en cas de défaillance d'une application, elle peut être rapidement redémarrée dans un nouveau conteneur sans affecter les autres applications. Les clusters de conteneurs peuvent également détecter automatiquement les conteneurs défaillants et les redémarrer.

**Load Balancing**

Le load balancing de charge consiste à distribuer le trafic réseau ou les demandes de manière équitable sur plusieurs serveurs ou ressources pour éviter la surcharge d'un seul point et améliorer la réactivité. Dans un environnement Docker, le load balancing peut être géré par Nginx, ou par des fonctionnalités intégrées dans des clusters de conteneurs.

**En quoi la clusterisation permet de répondre à ces problématiques ?**

La clusterisation permet la scalabilité horizontale, c'est-à-dire l'ajout de nœuds supplémentaires au cluster pour gérer l'augmentation de la charge. Cela est utile pour gérer les pics de trafic et la croissance à long terme.

Les clusters assurent une haute disponibilité en répliquant les services et les données sur plusieurs nœuds. En cas de défaillance d'un nœud, un autre peut prendre le relais, ainsi, le système reste opérationnel.

Les clusters permettent de répartir le trafic ou les requêtes de manière équilibrée entre les différents nœuds, assurant ainsi qu'aucun nœud unique ne soit surchargé.

**Faites une recherches sur des outils permettant d'orchestrer un cluster de conteneurs**

+ **Kubernetes** est un standard pour l'orchestration de conteneurs. Il offre une gestion automatisée de la scalabilité, de la disponibilité et de l'équilibrage de charge. Il est très flexible et peut être utilisé dans des environnements cloud, sur site ou hybrides.

+ **Docker Swarm** est intégré dans Docker et est idéal pour les utilisateurs qui préfèrent une solution plus simple et plus directe. Bien que moins riche en fonctionnalités que Kubernetes, Docker Swarm est plus facile à configurer et à utiliser, surtout pour ceux qui sont déjà familiers avec Docker.

+ **Apache Mesos** est conçu pour les environnements à grande échelle. Il offre une abstraction efficace des ressources du data center, permettant ainsi une gestion flexible des conteneurs et des charges de travail non conteneurisées.

+ **OpenShift** est une plateforme d'orchestration de conteneurs basée sur Kubernetes. Elle offre des fonctionnalités supplémentaires telles que la gestion des utilisateurs, la surveillance intégrée et des outils de développement pour faciliter le déploiement d'applications.


