<img width="1083" height="532" alt="image" src="https://github.com/user-attachments/assets/05723b5b-3e2f-4464-a3cf-2ea28f9c25c2" />

___________________
L'analyse du fichier `res/values/strings.xml` a permis d'identifier plusieurs éléments sensibles exposant l'infrastructure ou les utilisateurs.

___________________
**Tableau des vulnérabilités identifiées**

| Extrait du code | Risque associé |
| :--- | :--- |



La présence de clés API en clair dans les ressources XML est une faille de sécurité. Il est recommandé d'utiliser des variables d'environnement ou un coffre-fort numérique (Vault).
