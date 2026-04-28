<img width="1083" height="532" alt="image" src="https://github.com/user-attachments/assets/05723b5b-3e2f-4464-a3cf-2ea28f9c25c2" />

___________________
L'analyse du fichier `res/values/strings.xml` a permis d'identifier plusieurs éléments sensibles exposant l'infrastructure ou les utilisateurs.

___________________
**Tableau des vulnérabilités identifiées**

| Extrait du code | Risque associé |
| :--- | :--- |
| `<string name="google_api_key">AIzaSyBTgztvImsUfMWDa41PCrDWAj7dmyIDhUg</string>` | Élevé : Permet l'utilisation frauduleuse des services Cloud aux frais de l'entreprise. |
| `<string name="firebase_database_url">https://application-client-nickel.firebaseio.com/</string>` | Élevé : URL de la base de données Firebase. Permet de cibler des attaques d'injection ou d'exfiltration si les règles de sécurité sont mal configurées. |
| `ACCOUNT_ENDPOINT : https://api.nickel.eu/...` | Moyen : Divulgation des points d'entrée (endpoints) de l'API bancaire, facilitant le reverse-engineering du protocole de communication. |


