# Compatibilité — Android TV et Fire TV Stick

Essais du **8 novembre 2026**. Le même APK Android TV a été installé sur les deux appareils ci-dessous.

| Appareil vérifié | Système | Observations |
| --- | --- | --- |
| TCL Smart TV Pro | Android TV 12 (API 31) | Accueil, enregistrement SIP, vidéo du visiophone, fenêtre en coin, NVR et grille de quatre caméras. |
| Fire TV Stick AFTSS (`sheldon`) | Fire OS 7.6.5.2 (API 28) | Installation, interface TV, fenêtre d'appel au-dessus de l'accueil Amazon et de YouTube, NVR et grille de quatre caméras confirmés. |

L'application est conçue pour les appareils TV Android : elle requiert la fonction `android.software.leanback` et Android 8.0 au minimum. Un appareil sous **Vega OS** n'exécute pas les APK Android. Vérifiez le système du Fire TV Stick dans **Paramètres > Ma Fire TV > À propos** avant de télécharger.

## Ce qui dépend de l'installation

- **Fenêtre d'appel :** l'autorisation d'affichage par-dessus les autres applications est indispensable. Le comportement varie selon le fabricant et la version du système.
- **Notifications :** Fire OS peut masquer les notifications des applications tierces. Vérifiez l'appel avec la fenêtre et avec l'application ouverte.
- **SIP et RTSP :** certains visiophones n'acceptent qu'un enregistrement SIP ou qu'une session vidéo à la fois. Deux appareils surveillant le même visiophone peuvent se gêner.
- **NVR et grille :** ils ont fonctionné sur les deux appareils testés. Le nombre de flux simultanés qu'un autre appareil peut décoder dépend de son matériel et des profils vidéo du NVR.
- **Audio :** la piste sonore du flux, le micro disponible et l'interphonie bidirectionnelle doivent être vérifiés sur chaque installation. Le test du micro ne prouve pas qu'un appel peut être pris.
- **Frigate :** les canaux RTSP du NVR peuvent être les mêmes que ceux utilisés par Frigate. Une intégration directe à l'API Frigate et ses alertes ne sont pas confirmées par les éléments utilisés pour cette page.

## Installation et mises à jour

L'APK publié se trouve dans la [dernière release](https://github.com/crashcool69/Dahua-TV/releases/latest/download/DahuaTV.apk) sous le nom `DahuaTV.apk`. Sur Android TV **et** Fire TV, Downloader accepte le code **5492774**. Sur les deux systèmes, autorisez Downloader à installer des applications de source inconnue. Le [guide d'installation](INSTALLATION.md) détaille les chemins et la configuration.

Une mise à jour installée sur la version existante conserve normalement les réglages si l'APK garde la même signature. Désinstaller l'application efface ses données locales. Aucun mot de passe ne doit être ajouté au dépôt ou à une capture publique.
