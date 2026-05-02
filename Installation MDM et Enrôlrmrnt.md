# Créer un compte d'essai sur une solution comme Miradore ou ManageEngine Mobile Device Manager Plus #
# Cration de la règle du mot de passe à respecter #
Aller dans le menu Management/configuration profiles cliquer sur Add ensuite choisir Android 
 <img width="1472" height="622" alt="image" src="https://github.com/user-attachments/assets/622cc8cf-83a0-4db2-83b0-a5b5a4a6107f" />

 
 Ensuite selectionner Passcode
 <img width="1161" height="466" alt="image" src="https://github.com/user-attachments/assets/c558b9e4-f29a-4119-b454-87a65165c0c4" />

 Ensuite réglage du paramamétre du passcode à 12 caractères minimum en alphanumérique dans notre cas de test? Enfin nommé la règle
 <img width="742" height="428" alt="image" src="https://github.com/user-attachments/assets/821f1356-f2ff-40e8-89a6-b73a9870e26d" />

 <img width="604" height="267" alt="image" src="https://github.com/user-attachments/assets/d8f2aefd-97b4-4688-b9c6-35a61dce418b" />

 Verifier la règle dans la liste :
<img width="663" height="441" alt="image" src="https://github.com/user-attachments/assets/fc11e28f-46b9-41c2-937d-c85585ec9a79" />

<img width="958" height="521" alt="image" src="https://github.com/user-attachments/assets/607c8a4e-d470-46f8-bb60-b157ac7fb3d4" />

## Enrôlement du smartphone ##
Aller dans le menu Enrollment puis Android Entreprise dans le cas de notre test sur un téléphone personnel nous avons opté pour l'option " Fully managed with work profile" Cela va créer un conteneur sécurisé sur le smartphone,les applications personnelles restent privées, et les applications "Pro" sont marquées d'un petit cartable.

<img width="881" height="691" alt="image" src="https://github.com/user-attachments/assets/beb97194-88ba-40ae-8fb8-890fcdbcc5e6" />  



## Sur le smartphone ##

Télécharger l'application Miradore Online Client sur le Play Store ensuite scanner le QR-CODE 

Dans le cas d'un mobile profissionel avec un nom de domaine existant l'opération aurai terminé avec succès avec le scann du QR-code

Après avoir installer l'application sur le mobile personnel , celle ci n'offre pas la possibilité de scanner un QR-CODE et ne fourni pas de code pin pour pouvoir s'authtifier et ensuite enrôller, nous avons opté pour l'option compagny/user

<img width="1570" height="413" alt="image" src="https://github.com/user-attachments/assets/e71979ef-95fb-415d-95f5-fd4084c28062" />




Créer l'enrelôment avec envoi d'un code pin

<img width="1604" height="638" alt="image" src="https://github.com/user-attachments/assets/f9f2baac-76dc-4a1f-a0e3-257a7c192bc1" />
<img width="1618" height="577" alt="image" src="https://github.com/user-attachments/assets/42b0becb-4138-455f-874d-d991c33127b6" />
<img width="802" height="711" alt="image" src="https://github.com/user-attachments/assets/7122d869-a68e-4ffd-840e-e4ad3eb283dc" />



<img width="360" height="750" alt="image" src="https://github.com/user-attachments/assets/88122667-d82d-4fc0-ab1b-8b032540a58d" />
<img width="889" height="674" alt="image" src="https://github.com/user-attachments/assets/f8e358f9-0587-44ae-81b7-4a2ce8ff8318" />

## Option Emulateur: ##
Utiliser un émulateur est la méthode la plus propre car il sera considéré comme un appareil "neuf", ce qui permettra à Miradore d'en prendre le contrôle total sans conflit avec les données personnelles.
Nous avons opté pour Installation d'Android Studio une fois installer :

Cliquer sur le bouton "Create Device"

<img width="882" height="682" alt="image" src="https://github.com/user-attachments/assets/3496123e-7a23-4864-b8d9-1be4206ab3fc" />

Pour le "System Image", télécharger et sélectionner "Tiramisu" (Android 13)
<img width="1262" height="824" alt="image" src="https://github.com/user-attachments/assets/1fe31427-1c17-4ef8-aad0-c3d4d090861f" />


## Enrôlement MDM sur l'émulateur 
Une fois que l'émulateur est démarré  :
<img width="412" height="870" alt="image" src="https://github.com/user-attachments/assets/50afa04a-0864-4f1d-90a2-84ed23b2f526" />


L'emulateur plente pour des raison puisance processeur et RAM

# Tentative avec un Motorola remis à zero :

Installation de l'application Miradore online client,une fois l'application démarrée nous avons configuré un profil professional:

<img width="490" height="861" alt="image" src="https://github.com/user-attachments/assets/da39b9c0-a1aa-49ed-a42a-8257cbda1199" />
<img width="502" height="862" alt="image" src="https://github.com/user-attachments/assets/8e0da969-039b-42aa-82eb-26049925d247" />
<img width="430" height="826" alt="image" src="https://github.com/user-attachments/assets/bdf46516-f435-4104-81e4-862d4c025342" />



<img width="425" height="862" alt="image" src="https://github.com/user-attachments/assets/2830d942-82cf-47f0-9a78-b401586e8b78" />

Miradore exige le chiffrement des données pour mieux les sécurisées.

<img width="465" height="830" alt="image" src="https://github.com/user-attachments/assets/8784d4f9-7b66-46c0-9e7b-b9d181745984" />


Une fois les données chiffrées, l'étape suivante consiste à confugurer Miradore en acceptant les condition de collecte de données et autoriser la localisation esnuite la page de l'authentification.

<img width="458" height="860" alt="image" src="https://github.com/user-attachments/assets/5e454112-ed76-423c-8b9d-32c9c461a7c5" />




Le problème ne vient pas du TLS dans notre cas, mais plutôt du fait que Android 7  est devenu obsolète pour les solutions MDM modernes comme Miradore. Même si la couche TLS fonctionne techniquement (test sur le navigateur ), cette version d’Android ne supporte plus correctement certaines exigences actuelles du protocole d’enrôlement (API Android Enterprise, mécanismes d’authentification récents, gestion des profils de travail, politiques de sécurité renforcées). 

Résultat : le serveur refuse implicitement l’inscription du device ou ne parvient pas à finaliser le processus, ce qui se traduit côté client par une erreur générique d’authentification. En pratique, Android 7 n’est plus pleinement compatible avec les workflows MDM cloud récents, ce qui rend l’enrôlement instable voire impossible malgré une connectivité réseau et TLS fonctionnels.



































   











 




