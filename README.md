<p align="center"><img src="images/DahuaTV-glitch-anime.png" alt="Logo original Dahua TV" width="520"></p>

# Dahua TV

**Le visiophone et les caméras Dahua sur votre télévision.** Dahua TV reçoit les appels du portier, affiche sa vidéo dans une fenêtre sur l'écran et permet de consulter les caméras du NVR à la télécommande. L'application fonctionne sur le réseau local, sans service cloud obligatoire.

[Télécharger le dernier APK](https://github.com/crashcool69/Dahua-TV/releases/latest/download/DahuaTV.apk) · [Lire le guide d'installation](INSTALLATION.md) · [Voir la compatibilité](COMPATIBILITE.md)

## Découvrir l'application

L'accueil réunit le direct du visiophone, l'état de la surveillance SIP et les commandes principales. Lorsqu'un appel arrive, une petite fenêtre vidéo peut apparaître au-dessus de l'écran en cours, à condition que l'appareil autorise l'affichage par-dessus les autres applications.

![Capture réelle de l'accueil Dahua TV, vidéo et adresse locale floutées](images/accueil-floute.png)

L'onglet **Caméras** ouvre les flux du NVR. Vous pouvez choisir une caméra ou utiliser la grille de quatre caméras. Le NVR et cette grille ont été confirmés sur le Fire TV Stick testé, ainsi que sur la télévision TCL testée.

![Capture réelle de l'onglet Caméras, image et adresse locale floutées](images/nvr-floute.png)

Sur le Fire TV Stick testé, la fenêtre d'appel reste visible au-dessus de l'accueil Amazon. La partie filmée par le portier est floutée sur cette capture réelle.

![Capture réelle de la fenêtre d'appel sur Fire TV Stick, vue du portier floutée](images/fire-tv-appel-floute.png)

Les réglages couvrent le compte SIP du portier, le flux RTSP, les identifiants vidéo, la fenêtre d'appel et les canaux du NVR. Un bouton permet aussi de tester l'affichage de la fenêtre. Les données de votre installation se saisissent **sur votre appareil** : aucune adresse, aucun identifiant et aucun mot de passe personnel ne sont nécessaires dans ce dépôt.

## Matériel et fonctions

| Fonction | Ce qu'elle permet |
| --- | --- |
| VTO / VTH Dahua | Recevoir le signal d'appel du portier via un compte SIP adapté à votre installation. |
| Vidéo RTSP | Voir le direct du portier, puis la fenêtre d'appel si la superposition est autorisée. |
| NVR | Consulter les caméras et la grille de quatre flux sur les appareils vérifiés. |
| Frigate | Reprendre les flux RTSP du NVR utilisés dans une installation Frigate ; les éventuelles fonctions de détection dépendent de la version et de la configuration. |
| Télécommande | Parcourir l'accueil, les caméras et les paramètres sans écran tactile. |

## Installer Dahua TV

### Fire TV Stick : installation avec Downloader

1. Installez **Downloader** depuis l'Appstore Amazon.
2. Dans les paramètres du Fire TV Stick, **autorisez Downloader à installer des applications de source inconnue**.
3. Ouvrez Downloader et saisissez ce code :

```text
5492774
```

4. Téléchargez **`DahuaTV.apk`**, puis choisissez **Installer**.

Vous pouvez aussi ouvrir directement [le dernier APK](https://github.com/crashcool69/Dahua-TV/releases/latest/download/DahuaTV.apk) dans Downloader. Sur Android TV, il faut également autoriser l'application qui ouvre l'APK à installer des applications de source inconnue. Le [tutoriel illustré](INSTALLATION.md) détaille les deux parcours et la configuration du portier et des caméras.

## Compatibilité et limites

Le même APK a été vérifié le 8 novembre 2026 sur une **TCL Smart TV Pro sous Android TV 12** et un **Fire TV Stick AFTSS sous Fire OS 7.6.5.2**. Le NVR et la grille de quatre caméras fonctionnent aussi sur ce Fire Stick. Une TV ou un stick doit pouvoir installer des APK Android TV ; un appareil sous Vega OS ne peut pas exécuter cet APK. La fenêtre au-dessus des autres applications dépend des autorisations et du système de l'appareil.

Un portier peut limiter le nombre d'enregistrements SIP ou de sessions vidéo simultanés. Si la TV et le stick utilisent le même compte et le même flux, désactivez la surveillance continue sur l'un des deux si les appels ou l'image deviennent instables. La réception audio et la possibilité de parler au visiteur dépendent du flux, du matériel et de la version ; ne comptez pas sur une interphonie bidirectionnelle sans l'avoir testée sur votre installation. Consultez [les essais et limites connus](COMPATIBILITE.md).

Les captures ci-dessus proviennent de l'application réelle. Les zones privées y sont floutées ; aucune interface n'a été recréée pour cette page.
