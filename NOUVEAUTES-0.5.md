# Dahua TV 0.5 — les nouveautés

**Une nouvelle interface, trois sources de vidéo, la supervision du matériel, le portail et la mise à
jour depuis la TV.** Cette version s'installe par-dessus la précédente sans perdre les réglages.

## Une nouvelle interface

- **Des tuiles de verre** à la place des plaques plates : un corps qui s'assombrit vers le bas, une
  bande de lumière en haut et une ombre intérieure qui fait remonter le bas. Le relief ne demande
  aucun flou, donc rien ne ralentit la TV.
- **Une palette unique** sur les treize écrans : fond nuit, accent cyan, magenta pour les actions de
  la maison, vert pour la surveillance en ligne, rouge pour l'erreur et le hors ligne.
- **Un anneau de focus cyan** de 2 dp et un léger grossissement. Un bouton **choisi** est plein, un
  bouton seulement **survolé** reste teinté et cerclé : la télécommande ne fait plus passer un
  survol pour un choix. Le liseré n'est plus rogné par sa carte.
- **Le fond de vagues néon** n'habille plus que l'Accueil, les Caméras, la grille des quatre, le
  plein écran et la supervision. Les écrans de formulaire passent sur fond uni, où un champ se lit
  mieux.
- **Des tailles qui suivent l'écran** : l'interface garde ses proportions en 720p comme en 4K, sans
  rétrécir sur une TV à forte densité.
- **Un fondu de 160 ms** entre deux écrans, jamais de cadre blanc.
- **La pastille de surveillance ne clignote plus** : verte fixe quand le visiophone est enregistré,
  rouge immobile sinon. Seul le voyant `● EN DIRECT` clignote encore, parce qu'il annonce une image
  qui tourne vraiment.
- **Des boutons à la largeur de leur mot** : une action courte ne prend plus toute la ligne.

## Des paramètres par thème

- **Six thèmes** au lieu d'un rail : **Visiophone**, **Affichage**, **Maison**, **Diagnostic**,
  **Système**, **Aide**. Une bande d'onglets les porte, avec **Ko-fi** et **Enregistrer** à sa
  droite. Le thème consulté est retenu d'une visite à l'autre.
- **Plus de place pour les cartes** : plus de rail latéral ni de barre de pied, les réglages gagnent
  en largeur et en hauteur.
- **Un message en pastille** posé sur les cartes, effacé seul après six secondes, au lieu d'une
  ligne qui rognait le bas de l'écran.
- **Une aide en quatre cartes** : par où commencer, où trouver quoi, ce qui reste silencieux, ce que
  l'application ne fait pas. Toute la page tient sans défilement.

## Trois sources de vidéo au lieu d'une

- L'**accueil** et la **fenêtre en coin** peuvent afficher le visiophone, une **caméra libre** ou un
  **canal du NVR**, au choix dans **03 / SOURCE VIDÉO**. Le changement s'applique aussitôt, sans
  passer par **Enregistrer**.
- **L'accueil s'adapte** : le titre prend le nom de la caméra et le bouton de la porte devient
  **Afficher en fenêtre**, puisqu'il n'y a pas de porte à ouvrir sur une caméra. Le plein écran
  revient à l'accueil.
- **Une source supprimée** ne laisse pas un écran noir : la première source disponible prend sa
  place, et sans aucune source l'application l'écrit au lieu d'ouvrir un flux qui ne répondra pas.

### Caméras libres

- **Jusqu'à quatre caméras** d'une autre marque, pour un logement sans portier Dahua.
- **Sept marques proposées** — Dahua, Hikvision, Reolink, Tapo, Axis, Uniview et Autre — chacune
  avec le chemin de son flux principal et de son sous-flux.
- **L'écran construit l'adresse** à partir de ce que l'on connaît : la marque, l'adresse de la
  caméra, le compte et le mot de passe. Une **saisie avancée** accepte à la place une adresse RTSP
  complète.
- **L'adresse obtenue s'affiche pendant la frappe**, mot de passe masqué, et reste chiffrée sur la
  TV.

## Le NVR, de un à huit canaux

- **N'importe quel enregistreur Dahua** qui répond en RTSP : adresse, port du flux, port de
  l'interface web, compte, mot de passe, puis les canaux de **un à huit**.
- **Le direct ne se fige plus** sur les enregistreurs qui datent toutes leurs images au même
  instant : l'application rétablit le temps de chaque image avant de l'afficher.
- **Une mosaïque des quatre caméras** avec une image vivante sur chaque tuile, sans surcharger la
  TV. Une tuile qui échoue retente une fois et dit pourquoi si l'échec persiste. Toucher une tuile
  ouvre ce canal en plein écran, en haute définition.
- **Un garde-fou mémoire** : sur un appareil trop petit pour quatre images à la fois, la mosaïque est
  refusée avec la mesure affichée plutôt que de faire tomber la lecture.

## Firmware et santé des appareils

- **Un écran de supervision** qui lit, pour chaque appareil configuré, ce qu'il dit de lui-même :
  type, version de firmware, date de fabrication, cloud P2P, UPnP, Telnet et horloge NTP.
- **Chaque appareil porte une puce** : **CONFORME**, **À CORRIGER** quand un réglage risqué est
  actif ou quand le firmware a plus de trois ans, **NON LISIBLE** ou **INJOIGNABLE**. Une valeur
  inconnue n'est jamais présentée comme conforme.
- **Un relevé qui se souvient** : un changement de firmware entre deux vérifications est annoncé.
- **Tout est en lecture seule** : l'application ne modifie aucun réglage et n'essaie aucun mot de
  passe.

## Portail et portique

- **Un nouvel écran** pour ouvrir, fermer ou arrêter un portail motorisé, depuis la TV.
- **Une box Somfy sur le réseau local** : rien ne passe par le cloud, la coupe d'internet ne coupe
  pas le portail.
- **Une connexion par jeton** de développement, sans jamais transmettre un compte Somfy à la box.
- **Des commandes confirmées** : une confirmation dit ce qui va se passer, puis un **pavé à quatre
  chiffres** à trois essais si un code a été enregistré pour le portail.
- **Un compte rendu honnête** : l'ordre accepté, son exécution terminée ou refusée, et la position
  relue. Une commande acceptée n'est jamais présentée comme un portail ouvert, et l'état reste
  **INCONNU** quand la box ne rapporte pas la position.
- **Seuls les boutons utiles** sont dessinés : un portail sans arrêt intermédiaire ne reçoit pas de
  bouton **Stop**.

## Sauvegarde de la configuration

- **Export et import en un seul fichier**, écrit dans les Téléchargements de la TV ou d'une clé
  branchée, pour retrouver toute sa configuration après une réinstallation ou sur une TV neuve.
- **Les mots de passe restent chiffrés** : ils reviennent lisibles après une mise à jour et
  reviennent vides après une réinstallation, la clé de la TV ayant disparu avec l'application. Les
  autres réglages, eux, sont bien transportés.

## Mise à jour depuis la TV

- **La carte MISE À JOUR** interroge la release publiée, compare son numéro à la version installée,
  télécharge l'APK et passe la main à l'installateur d'Android. Plus besoin d'un ordinateur.
- **Un bandeau sur l'accueil** signale une version plus récente quand il y en a une.
- **L'état de l'autorisation** d'installer une application est affiché en clair sur cette même
  carte.

## Le reste, en plus court

- La **langue** se choisit en **Auto**, **Français** ou **English**, et tous les nouveaux écrans
  suivent ce choix.
- La tuile **SIGNATURE** de l'accueil ouvre la page du projet, tout comme le bouton **Ko-fi** des
  Paramètres.
- La **grille des quatre caméras** et l'**historique des appels** sont désormais accessibles depuis
  les mêmes écrans que le reste, avec les mêmes cartes et les mêmes boutons.

L'APK se trouve dans la [dernière release](https://github.com/crashcool69/Dahua-TV/releases/latest).
