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

Dans le cas d'un mobile profissionel 

<img width="1570" height="413" alt="image" src="https://github.com/user-attachments/assets/e71979ef-95fb-415d-95f5-fd4084c28062" />

Après avoir installer l'application sur le mobile personnel , celle ci n'offre pas la possibilité de scanner un QR-CODE et ne fourni pas de code pin pour pouvoir s'authtifier et ensuite enrôller, nous avons opté pour l'option compagny/user


Créer l'enrelôment avec envoi d'un code pin

<img width="1604" height="638" alt="image" src="https://github.com/user-attachments/assets/f9f2baac-76dc-4a1f-a0e3-257a7c192bc1" />
<img width="1618" height="577" alt="image" src="https://github.com/user-attachments/assets/42b0becb-4138-455f-874d-d991c33127b6" />
<img width="704" height="469" alt="image" src="https://github.com/user-attachments/assets/70979bdf-a14f-47ad-8833-2eec80836774" />

Un username a bien été crée avec un pin mais l'enrelement a échoué sur un smatphone personnel.
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



Le "Secret" Android Enterprise : Ne cliquer pas sur "Démarrer". Tapoter 7 fois très vite sur une zone vide de l'écran.

Cela va activer le scanner de QR Code caché.

Android demander de te connecter au Wi-Fi. (L'émulateur se connectera au Wi-Fi virtuel "AndroidWifi").

Une fois connecté, l'appareil photo de l'émulateur va s'ouvrir.

Scan : Utiliser la webcam du PC pour scanner le QR Code de Miradore celui du mode Fully Managed .

Astuce : Si tu n'as pas de webcam, tu peux copier le lien de l'image du QR code dans le navigateur de l'émulateur.

4. Validation finale
L'émulateur va dire : "Cet appareil appartient à votre organisation".

Il va installer automatiquement l'application Miradore.

Capture d'écran 1 : L'émulateur affichant "Appareil géré".

Capture d'écran 2 : Dans ta console Miradore sur Kali, ton émulateur apparaîtra enfin dans Devices.



xxdqs


qsdqD





























   











 




