<div align="center">

<img src="assets/icon.png" width="128" alt="Icône Slide">

# Slide

**Glissez un fichier, un lien, une note ou un message vers un autre Mac, c'est envoyé.**
Même pièce, même Wi-Fi. Rien à configurer, aucun compte, aucun serveur.

[![Télécharger Slide pour Mac](https://img.shields.io/badge/T%C3%A9l%C3%A9charger-Slide.dmg-5B6CFF?style=for-the-badge&logo=apple&logoColor=white)](https://github.com/Lascages/slide-releases/releases/latest/download/Slide.dmg)

![version](https://img.shields.io/github/v/release/Lascages/slide-releases?style=flat-square&color=5B6CFF&label=derni%C3%A8re%20version)
![macOS](https://img.shields.io/badge/macOS-13%2B-1f2937?style=flat-square&logo=apple)
![architectures](https://img.shields.io/badge/Apple%20Silicon%20%2B%20Intel-1f2937?style=flat-square)
![mises à jour](https://img.shields.io/badge/mises%20%C3%A0%20jour-automatiques-2DD4A3?style=flat-square)
![chiffré](https://img.shields.io/badge/transferts-chiffr%C3%A9s-9B5CFF?style=flat-square)

[Installation](#installation) · [Premiers pas](#premiers-pas) · [Envoyer](#envoyer) · [Recevoir](#recevoir) · [Mises à jour](#mises-à-jour) · [Sécurité](#sécurité-et-confidentialité) · [Dépannage](#dépannage)

</div>

---

> [!IMPORTANT]
> **Les deux personnes doivent avoir Slide ouvert**, sur le même réseau Wi-Fi (ou le même câble). Envoyez-leur simplement le lien de téléchargement ci-dessus.

## Installation

1. **Téléchargez** [Slide.dmg](https://github.com/Lascages/slide-releases/releases/latest/download/Slide.dmg) et ouvrez-le.
2. **Glissez Slide dans Applications**, puis lancez-le.
3. **Premier lancement uniquement** : macOS affiche un avertissement, car Slide n'est pas encore validée par Apple. C'est normal.
   - Ouvrez **Réglages Système > Confidentialité et sécurité**, descendez jusqu'à « Slide a été bloqué », cliquez **Ouvrir quand même**, puis confirmez.
   - *Ou, en une commande dans le Terminal :*
     ```bash
     xattr -dr com.apple.quarantine /Applications/Slide.app
     ```

Ensuite, **Slide se met à jour tout seul** : vous n'aurez plus jamais à retélécharger quoi que ce soit.

**Configuration requise** : macOS 13 (Ventura) ou plus récent · Mac Apple Silicon (M1 et suivants) ou Intel.

## Premiers pas

1. Lancez Slide sur **les deux Macs**.
2. Acceptez les autorisations demandées (voir le tableau ci-dessous).
3. Chaque Mac apparaît chez l'autre en quelques secondes.
4. **Glissez un fichier** vers la personne : c'est parti.

| Autorisation | Pourquoi | Quand |
|---|---|---|
| **Réseau local** | Trouver les autres Macs et leur envoyer des données | Au premier lancement |
| **Notifications** | Être prévenu d'une demande ou d'un envoi terminé | Au premier lancement |
| **Automatisation > Notes** | Lire une note que vous glissez, ou l'ajouter dans Notes à la réception | Au premier envoi ou à la première réception d'une note |
| **Automatisation > navigateur** | Envoyer la page ouverte dans Safari, Chrome, Brave, Arc ou Edge | À la première utilisation de « envoyer la page du navigateur » |
| **Bureau / Documents** | Envoyer automatiquement vos captures d'écran (option) | Si vous activez cette option |

> [!TIP]
> Dans **Réglages**, lancez la **notification de test** pour vérifier que tout s'affiche, et activez **Lancer au démarrage** pour ne manquer aucune demande.

## Envoyer

### Les façons d'envoyer

| Façon | Comment |
|---|---|
| **Glisser-déposer** | Commencez à glisser n'importe quoi : une cible apparaît pour chaque Mac détecté, relâchez dessus |
| **Dans la fenêtre Slide** | Glissez sur la carte d'un Mac, ou cliquez **Envoyer…** et choisissez les fichiers |
| **Clic droit sur un Mac** | Fichiers, message, presse-papiers, page du navigateur, « regarder ensemble » |
| **Raccourci `⌃⌥⌘S`** | Envoie votre presse-papiers (texte, image, fichier…) |
| **Raccourci `⌃⌥⌘B`** | Envoie la page ouverte dans votre navigateur |
| **Captures d'écran** | Réglages > envoi automatique de vos nouvelles captures vers le Mac de votre choix |

### Ce que vous pouvez envoyer, et ce qui se passe chez l'autre

| Vous envoyez | Chez le destinataire |
|---|---|
| **Fichiers et dossiers** | Enregistrés dans `Téléchargements/Slide`, avec une tuile à glisser où on veut |
| **Lien** | Après acceptation, **ouvert directement dans son navigateur principal** |
| **Lien YouTube** | Idem, avec l'horodatage conservé et la lecture automatique demandée *(le navigateur peut la refuser, Chrome et Brave la permettent en général)* |
| **Lien Spotify, Apple Music, Zoom, Teams, Notion, Figma** | Ouvert **dans l'app native** si elle est installée |
| **Note Apple Notes** | **Recréée dans son app Notes**, avec la mise en forme |
| **Texte, image, PDF** | Copiés dans son presse-papiers, avec une tuile |
| **Contact `.vcf`, événement `.ics`** | Enregistrés, avec un bouton **Ouvrir** |
| **Message court** | Affiché en bannière, avec un bouton **Répondre…** |
| **Regarder ensemble** | La vidéo démarre **au même instant** sur les deux Macs (6 secondes après l'envoi) |

## Recevoir

Quand quelqu'un vous envoie quelque chose, **une boîte de confirmation s'affiche au premier plan**, même si la fenêtre Slide est fermée ou si vous êtes en plein écran. Elle montre :

- **qui** envoie : son nom, le modèle de son Mac, son adresse et sa position ;
- **quoi** : les fichiers avec leur taille, l'aperçu du texte, le lien, le titre de la note ;
- **ce qui se passera** : le bouton s'adapte (« Accepter et ouvrir », « Accepter et ajouter à Notes »…).

Vous pouvez aussi répondre **depuis la notification**, avec les boutons *Accepter*, *Toujours accepter* et *Refuser*. Sans réponse après 90 secondes, la demande est refusée.

**Macs de confiance** : cochez *Toujours accepter les envois de…* pour ne plus avoir de confirmation avec cette personne. Gérez la liste dans Réglages > Sécurité.

**Suivre ce qui se passe** : l'onglet **Activité** liste chaque transfert avec son statut détaillé (*En attente d'acceptation*, *Lien ouvert dans le navigateur*, *Note ajoutée à Notes*, *Refusé*, *Injoignable*…) et des boutons *Ouvrir le lien* ou *Afficher*. Chaque événement (accepté, refusé, reçu, échec, Mac à proximité…) déclenche aussi une bannière.

## Mises à jour

- **Automatiques** : Slide vérifie toutes les heures, télécharge et s'installe tout seul.
- **À la demande** : *Slide > Rechercher les mises à jour…*, ou Réglages > Mises à jour.
- **Versions bêta** : Réglages > *Recevoir aussi les versions bêta* pour tester les nouveautés en avance.
- Chaque mise à jour est **signée** : Slide refuse toute mise à jour qui ne vient pas de nous.

Toutes les versions sont dans l'onglet [Releases](https://github.com/Lascages/slide-releases/releases).

## Sécurité et confidentialité

- **Aucun serveur, aucun compte** : les Macs échangent **directement** entre eux, sur votre réseau. Rien ne passe par internet.
- **Tout est chiffré** (TLS avec clé partagée) : un tiers sur le même Wi-Fi ne peut pas lire les transferts.
- **Code de la pièce** *(optionnel, Réglages > Sécurité)* : définissez le même mot de passe sur vos Macs, et seuls ceux-là se voient et se parlent.
- **Rien n'arrive sans votre accord** : chaque envoi d'un Mac inconnu demande une confirmation.
- **Le contenu de vos fichiers n'est jamais lu en dehors de l'envoi**. Slide ne regarde que ce que vous glissez ou envoyez.

## Dépannage

<details>
<summary><b>Je ne vois pas l'autre Mac</b></summary>

- Slide est-il **ouvert sur les deux** Macs ?
- Même réseau Wi-Fi ? Un Wi-Fi « invité » isole souvent les appareils : essayez un autre réseau, un partage de connexion, ou un câble.
- **Réglages Système > Confidentialité et sécurité > Réseau local** : Slide doit être activé.
- Le **pare-feu** macOS ne doit pas bloquer les connexions entrantes de Slide.
- Si vous avez défini un **code de la pièce**, il doit être identique des deux côtés.
- En dernier recours : Réglages > **Connexion manuelle** (saisissez l'adresse IP de l'autre Mac).
</details>

<details>
<summary><b>macOS refuse d'ouvrir Slide</b></summary>

C'est l'avertissement du premier lancement (voir [Installation](#installation)) : **Ouvrir quand même** dans Confidentialité et sécurité, ou la commande `xattr` du Terminal.
</details>

<details>
<summary><b>Je ne vois pas les bannières</b></summary>

Les bannières Slide s'affichent toujours en haut à droite. Pour celles de macOS : Réglages Système > Notifications > Slide, style « Bannières » ou « Alertes ». Le mode Concentration masque les notifications macOS, mais jamais la boîte de confirmation. **Réglages > Notifications** affiche l'état exact et propose un test.
</details>

<details>
<summary><b>Une note ne s'ajoute pas dans Notes</b></summary>

Autorisez Slide à contrôler Notes : Réglages Système > Confidentialité et sécurité > **Automatisation** > Slide > Notes. Le journal (Réglages) indique la raison exacte en cas d'échec.
</details>

<details>
<summary><b>La vidéo YouTube ne démarre pas toute seule</b></summary>

Slide demande la lecture automatique, mais **c'est le navigateur qui décide**. Chrome et Brave l'autorisent en général, Safari la bloque souvent : dans Safari, Réglages > Sites web > Lecture automatique.
</details>

<details>
<summary><b>Quelque chose ne marche pas et je ne sais pas pourquoi</b></summary>

Ouvrez **Réglages > Journal** : chaque envoi, réception et échec y est noté avec sa cause. Cliquez *Copier le journal* et envoyez-le nous, ou ouvrez une [issue](https://github.com/Lascages/slide-releases/issues).
</details>

## Bientôt

- Comptes et **organisations** : envoyer à vos contacts et collègues, même sur un autre réseau.
- Une liste de personnes classée par fréquence d'échange, puis par organisation.
- Envoi à une **équipe** entière en un glisser.

---

<div align="center"><sub>Slide · fait avec soin · le code source est privé, les versions sont publiques</sub></div>
