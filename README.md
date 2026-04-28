Voici les métadonnées de l'application : 

App Name: Nickel

Package Name: com.fpe.comptenickel

Main Activity: com.fpe.comptenickel.MainActivity

Target SDK: 28

Min SDK: 19

Max SDK:

Android Version Name: 2.12.0

Android Version Code: 150

____________________________

Voici la liste des vulnérabilités : 

**Janus Vulnerability**

Gravité : Warning

Description :
L'application est signée avec APK Signature Scheme v1 uniquement
Cela la rend vulnérable à la Janus vulnerability

Impact :
Permet d’injecter du code malveillant dans un APK signé
Affecte Android 5.0 → 8.0

Cause :
Absence de Signature Scheme v2/v3

Recommandation :
Signer avec APK Signature Scheme v2 ou v3


**Cryptographie faible** 

Gravité : Warning

Problème :
Utilisation de MD5

Références :
CWE-327 : Use of Broken Cryptographic Algorithm
OWASP Mobile Top 10 : M5 Insufficient Cryptography

Exemples de fichiers concernés :

RNFetchBlobUtils.java
RNFetchBlobBody.java
PushBundleStorageImpl.java

Impact :
MD5 vulnérable aux collisions
Risque de bypass d’intégrité ou signature

Recommandation :
Remplacer par SHA-256 / SHA-3
