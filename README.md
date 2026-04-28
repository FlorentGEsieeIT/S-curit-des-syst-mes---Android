### Recomplication de l'APK ###
apktool b app -o rebuilt.apk
<img width="673" height="325" alt="image" src="https://github.com/user-attachments/assets/e77649b8-eb47-4657-aecd-bc92ea22717d" />
### Signature de l'APK ###
   # 1. Génération de la clé Keystore #
   Command Line: keytool -genkey -v -keystore lab-key.jks -keyalg RSA -keysize 2048 -validity 10000 -alias nickel-alias

   <img width="1111" height="343" alt="image" src="https://github.com/user-attachments/assets/73640844-aecf-45ca-8af9-78900dc9cc1d" />

  # Signature de l'APK
  Command line : apksigner sign --ks lab-key.jks --out rebuilt_signed.apk rebuilt.apk
<img width="840" height="399" alt="image" src="https://github.com/user-attachments/assets/d086a6e8-35cc-4302-9634-225130079752" />

