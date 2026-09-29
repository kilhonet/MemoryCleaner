# MemoryCleaner

**Un nettoyeur de mémoire léger et gratuit pour Windows : il libère la mémoire d'un clic et nettoie tout seul selon les conditions que vous fixez.**

[English](README.md) · [한국어](README.ko.md) · [简体中文](README.zh-CN.md) · [日本語](README.ja.md) · [Español](README.es.md) · [Português (Brasil)](README.pt-BR.md) · Français

> Ce document est une traduction. En cas de différence, la [version coréenne](README.ko.md) fait foi.

![Platform](https://img.shields.io/badge/platform-Windows%2010%20%2F%2011%20(64--bit)-0078D4)
![License](https://img.shields.io/badge/license-Freeware-brightgreen)
![Version](https://img.shields.io/badge/version-3.0.0-blue)
[![Download](https://img.shields.io/badge/download-kilho.net-orange)](https://down.kilho.net/memorycleaner?lang=fr)

![Écran de MemoryCleaner](images/memorycleaner-en.webp)

## Présentation

MemoryCleaner montre combien de mémoire est utilisée en ce moment, et un seul clic sur **Nettoyer la mémoire** récupère le cache que Windows garde en réserve et la mémoire que les programmes ouverts n'utilisent pas pour l'instant.

Vous pouvez lui demander de nettoyer tout seul quand l'utilisation de la mémoire devient élevée, à intervalle régulier, ou quand le cache s'accumule et que la mémoire libre vient à manquer. Pendant qu'un jeu ou une vidéo tourne en plein écran, il saute le nettoyage pour ne jamais vous gêner.

Fermer la fenêtre l'envoie dans la zone de notification (barre d'état système), où il continue à travailler discrètement. Une fois la fenêtre fermée, MemoryCleaner libère aussi toute la mémoire qu'elle utilisait : en attente dans la barre d'état, il n'occupe lui-même qu'environ 1 Mo.

## Fonctionnalités

- **Nettoyage en un clic** — Nettoyez la mémoire avec le bouton **Nettoyer la mémoire** ou d'un simple clic sur l'icône de la barre d'état.
- **Choix des zones à nettoyer** — Choisissez vous-même les zones : cache de fichiers, ensemble de travail, liste de veille, cache du registre, combinaison de la mémoire, etc.
- **Nettoyage automatique** — Nettoie quand l'utilisation de la mémoire physique · virtuelle · de l'ensemble de travail dépasse un seuil, ou à intervalle régulier.
- **Anti-saccades en jeu** — Quand le cache (la liste de veille) s'accumule et que la mémoire libre manque, il vide uniquement le cache.
- **Détection du plein écran** — Saute le nettoyage automatique pendant qu'un jeu, une vidéo ou une présentation est en plein écran.
- **État de la mémoire** — Mémoire physique, mémoire virtuelle, ensemble de travail et cache sur l'écran d'accueil et l'icône de la barre d'état.
- **Léger** — Un seul exécutable, qui n'occupe qu'environ 1 Mo en attente dans la barre d'état.
- **9 langues** — Coréen · anglais · japonais · chinois · russe · italien · français · espagnol · arabe.

## Téléchargement / Installation

| Type | Lien |
|---|---|
| Version à installer | [Télécharger](https://down.kilho.net/memorycleaner?lang=fr) |
| Version portable (ZIP) | [Télécharger](https://down.kilho.net/memorycleaner?lang=fr&nosetup) |

La version à installer lance MemoryCleaner dès la fin de l'installation et active **Lancer au démarrage** : il démarre dans la barre d'état à chaque ouverture de session Windows. Pour la version portable, décompressez le ZIP et lancez `MemoryCleaner.exe`. Les deux versions ont les mêmes fonctions.

Nettoyer la mémoire nécessite les droits d'administrateur : Windows affiche donc une demande d'autorisation au lancement. Cliquez sur **Oui**.

## Utilisation

### Premiers pas

1. Lancez MemoryCleaner et cliquez sur **Oui** dans la demande d'autorisation d'administrateur.
2. **Accueil** affiche l'utilisation de la mémoire physique sous forme de barre et de chiffres, avec en dessous la mémoire virtuelle · l'ensemble de travail · le cache. Les valeurs se mettent à jour chaque seconde.
3. Cliquez sur **Nettoyer la mémoire** : le bouton devient **Nettoyage en cours**, et une fois terminé vous voyez aussitôt la baisse de l'utilisation.
4. Pour qu'il nettoie tout seul, cliquez sur **Config** et activez les conditions voulues sous **Nettoyage automatique**.
5. Fermer la fenêtre laisse MemoryCleaner actif dans la barre d'état. Cliquez sur l'icône pour rouvrir la fenêtre.

### Organisation de l'écran

**Boutons du haut**

| Élément | Rôle |
|---|---|
| **Accueil** | L'écran principal, avec l'état de la mémoire et le bouton **Nettoyer la mémoire** |
| **Config** | Nettoyage automatique · Zones à nettoyer · Général |
| **Donner** | Ouvre la page de don |
| Logo KILHO.net | Ouvre la page de présentation de MemoryCleaner |

**Accueil**

| Élément | Contenu |
|---|---|
| Barre | Utilisation de la mémoire physique |
| **Physique** | Utilisée / totale (Mo) et taux d'utilisation |
| **Virtuelle** | Utilisation de la mémoire virtuelle, fichier d'échange compris |
| **Travail** | Mémoire occupée par les programmes ouverts, et sa part |
| **Cache** | Mémoire que Windows garde en cache (la même valeur que « En cache » dans le Gestionnaire des tâches) et sa part de la mémoire physique |
| **Nettoyer la mémoire** | Nettoie tout de suite. Devient **Nettoyage en cours** pendant le travail |

**Config**

| Groupe | Éléments |
|---|---|
| **Nettoyage automatique** | **Mémoire physique (%) : Nettoyer si utilisation dépasse.** · **Fichier de pagination (%) : Nettoyer si utilisation dépasse.** · **Ensemble de travail (%) : Nettoyer si utilisation dépasse.** · **Nettoyer quand l'intervalle (minutes) dépasse.** · **Vider le cache (liste de veille) (anti-saccades)** · **Ne pas nettoyer en plein écran** |
| **Zones à nettoyer** | **Cache de fichiers** · **Travail** · **Liste de veille (basse priorité)** · **Cache du registre** · **Combiner la mémoire** · **Liste de veille \*** · **Liste des pages modifiées \*** |
| **Général** | **Lancer au démarrage** · **Cliquez sur l'icône de la barre pour nettoyer.** |
| En bas | Version actuelle et bouton **Par défaut** |

**Icône de la barre d'état**

| Action | Résultat |
|---|---|
| Survol | Utilisation de la mémoire physique · virtuelle · de l'ensemble de travail |
| Clic gauche | Ouvre la fenêtre (nettoie aussitôt si **Cliquez sur l'icône de la barre pour nettoyer.** est activé) |
| Clic droit | **Nettoyeur** (ouvrir la fenêtre) · **Créé par Kilho** (page de présentation) · **Quitter** |

Pendant le nettoyage, l'icône change d'aspect : vous savez qu'il travaille sans ouvrir la fenêtre.

**Zones à nettoyer** — ce que chacune libère

| Élément | Ce qui est libéré | Par défaut |
|---|---|---|
| **Cache de fichiers** | Le cache que Windows accumule en lisant et en écrivant des fichiers | Activé |
| **Travail** | La mémoire que les programmes ouverts n'utilisent pas pour l'instant | Activé |
| **Liste de veille (basse priorité)** | La partie du cache la moins susceptible de resservir | Activé |
| **Cache du registre** | Le cache accumulé en lisant le registre | Activé |
| **Combiner la mémoire** | Regroupe les contenus de mémoire identiques en un seul pour faire de la place | Activé |
| **Liste de veille \*** | Tout le cache | Désactivé |
| **Liste des pages modifiées \*** | La mémoire en attente d'écriture sur le disque | Désactivé |

Les éléments marqués `*` peuvent provoquer de brèves saccades en jeu ou pendant une vidéo ; ils sont donc désactivés au départ.

### Que faire quand…

**Nettoyer la mémoire tout de suite**
Cliquez sur **Nettoyer la mémoire** dans **Accueil**. Le bouton devient **Nettoyage en cours** pendant le travail, puis redevient **Nettoyer la mémoire**. Cliquez-y une fois quand votre PC s'alourdit après avoir laissé beaucoup de programmes ouverts, ou juste avant de lancer un gros jeu ou un logiciel de montage.

**Nettoyer depuis l'icône sans ouvrir la fenêtre**
Activez **Config → Cliquez sur l'icône de la barre pour nettoyer.** : un simple clic sur l'icône nettoie la mémoire. À la fin, la notification « Mémoire optimisée. » s'affiche. Tant que ce réglage est activé, ouvrez la fenêtre par un clic droit sur l'icône → **Nettoyeur**.

**Voir l'état de la mémoire sans la fenêtre**
Survolez l'icône de la barre d'état pour voir l'utilisation de la mémoire physique · virtuelle · de l'ensemble de travail — de quoi juger s'il faut nettoyer sans ouvrir la fenêtre.

**Nettoyer automatiquement quand la mémoire manque**
Sous **Config → Nettoyage automatique**, activez **Mémoire physique (%) : Nettoyer si utilisation dépasse.** et choisissez un seuil (30 – 90 %) dans la case à côté. Dès que l'utilisation dépasse le seuil, MemoryCleaner nettoie tout seul. Si vous sollicitez beaucoup le fichier d'échange, activez aussi **Fichier de pagination (%) : Nettoyer si utilisation dépasse.** ; si ce sont les programmes gourmands en mémoire qui posent problème, activez **Ensemble de travail (%) : Nettoyer si utilisation dépasse.**. Quand le nettoyage ne fait pas baisser l'utilisation, il attend avant de recommencer au lieu de nettoyer en boucle, pour que le nettoyage ne devienne pas lui-même une charge.

**Nettoyer à intervalle régulier**
Activez **Nettoyer quand l'intervalle (minutes) dépasse.** et choisissez 5 · 10 · 20 · 30 · 40 · 50 · 60 minutes : il nettoie alors à cet intervalle, quelle que soit l'utilisation. Pratique pour garder léger un PC qui reste allumé longtemps.

**Quand un jeu devient de plus en plus saccadé au fil de la partie (vider le cache)**
Il arrive qu'un jeu saccade de plus en plus au fil du temps, jusqu'à ce que seul un redémarrage du jeu règle le problème. C'est que Windows garde les fichiers déjà lus en cache (la liste de veille) ; quand ce cache s'accumule et que la mémoire libre s'épuise, Windows doit le récupérer en urgence, ce qui fige le jeu un instant. Activez **Vider le cache (liste de veille) (anti-saccades)** : quand le cache dépasse le seuil **Vider si le cache (Mo) dépasse** (512 · 1024 · 2048 · 4096 Mo) et qu'en même temps la mémoire libre passe sous le seuil **Vider si la mémoire libre (Mo) est sous** (1024 · 2048 · 4096 · 8192 · 16384 Mo), il vide uniquement le cache à l'avance. Il n'agit que si les deux conditions sont réunies, et une fois le cache vidé elles disparaissent d'elles-mêmes : il n'intervient que quand c'est utile.

Le mieux est de régler le seuil de mémoire libre sur la moitié de la mémoire installée dans votre PC.

| Mémoire installée | Vider si la mémoire libre (Mo) est sous |
|---|---|
| 8 Go | 4096 (par défaut) |
| 16 Go | 8192 |
| 32 Go | 16384 |

Inutile de ne l'activer que pour jouer. Il n'occupe qu'environ 1 Mo dans la barre d'état et n'agit que quand les conditions sont réunies : laissez-le simplement activé.

**Ne rien toucher pendant un jeu ou un film**
**Ne pas nettoyer en plein écran** est activé d'emblée. Pendant qu'un jeu, une vidéo ou une présentation est en plein écran, le nettoyage automatique est sauté pour éviter toute saccade. Une fois sorti du plein écran, il reprend normalement.

**Choisir soi-même les zones à nettoyer**
Cochez les zones à nettoyer sous **Config → Zones à nettoyer**. Le bouton **Nettoyer la mémoire** comme le nettoyage automatique suivent ces choix. Si rien n'est coché, il n'y a rien à faire : le bouton **Nettoyer la mémoire** est grisé.

**Pour un nettoyage plus poussé**
Activer **Liste de veille \*** et **Liste des pages modifiées \*** libère aussi tout le cache et la mémoire en attente d'écriture : c'est ce qui libère le plus de mémoire. Cela peut toutefois provoquer de brèves saccades en jeu ou pendant une vidéo ; activez-les seulement au besoin et laissez-les désactivés le reste du temps.

**Ce que signifie « Cache »**
**Cache** dans **Accueil** est la mémoire que Windows garde au cas où elle resservirait — la même valeur que « En cache » dans le Gestionnaire des tâches. Une valeur élevée n'est pas mauvaise en soi, mais si vos jeux saccadent, essayez d'activer le vidage du cache ci-dessus.

**Démarrer automatiquement avec Windows**
Activez **Config → Lancer au démarrage** : peu après l'ouverture de votre session Windows, MemoryCleaner démarre discrètement dans la barre d'état — sans demande d'autorisation d'administrateur. C'est activé d'emblée dans la version installée.

**Le garder actif après avoir fermé la fenêtre**
Le X de la fenêtre ne quitte pas MemoryCleaner : il passe dans la barre d'état et continue le nettoyage automatique. Il libère alors aussi toute la mémoire de la fenêtre, si bien que le laisser tourner ne coûte presque rien. Pour quitter complètement, faites un clic droit sur l'icône → **Quitter** et confirmez.

**Quitter pendant un nettoyage**
Si vous quittez pendant un nettoyage, le bouton devient **Quitter après le nettoyage**, et le programme se ferme une fois le nettoyage terminé. Le nettoyage n'est jamais interrompu en cours de route.

**Rétablir tous les réglages**
Cliquez sur **Par défaut** en bas de **Config** et confirmez : tous les réglages de nettoyage automatique et de zones à nettoyer reviennent à leurs valeurs par défaut. **Lancer au démarrage** n'est pas modifié.

**Le relancer alors qu'il tourne déjà**
Un seul MemoryCleaner fonctionne à la fois. Le relancer alors qu'il est dans la barre d'état n'en démarre pas un nouveau : la fenêtre de celui qui tourne déjà s'ouvre.

## Configuration

Chaque réglage est enregistré dès que vous le modifiez et réutilisé au prochain lancement.

| Élément | Par défaut |
|---|---|
| Nettoyage selon l'utilisation de la mémoire physique · du fichier de pagination · de l'ensemble de travail | Désactivé (seuil de 90 % une fois activé) |
| Nettoyer quand l'intervalle (minutes) dépasse. | Désactivé (30 minutes une fois activé) |
| Vider le cache (liste de veille) | Désactivé (cache ≥ 1024 Mo · mémoire libre < 4096 Mo une fois activé) |
| Ne pas nettoyer en plein écran | Activé |
| Zones à nettoyer | Cache de fichiers · Travail · Liste de veille (basse priorité) · Cache du registre · Combiner la mémoire |
| Lancer au démarrage | Activé dans la version installée |
| Cliquez sur l'icône de la barre pour nettoyer. | Désactivé |
| Langue | Suit le paramètre de région de Windows (anglais si la langue n'est pas prise en charge) |

## Configuration requise

- Windows 10 · Windows 11 (64 bits)
- Droits d'administrateur — nécessaires pour nettoyer la mémoire. Une demande d'autorisation s'affiche au lancement (mais pas au démarrage via **Lancer au démarrage**).
- Aucun autre composant à installer.
- La connexion Internet ne sert qu'aux avis de nouvelle version.

## Mises à jour

MemoryCleaner ne se met **pas** à jour tout seul. Au démarrage, il vérifie s'il existe une nouvelle version et affiche un avis ; cliquer sur **[Oui]** ouvre la page de téléchargement et ferme le programme. Les nouvelles versions sont publiées manuellement après des tests internes et annoncées sur la [page de MemoryCleaner](https://kilho.net/memorycleaner). Consultez l'[avis sur la politique de mise à jour](https://en.kilho.net/archives/notice/2940).

**Historique des versions**

| Version | Date | Modifications |
|---|---|---|
| 3.0.0 | 2026-09-29 | Entièrement refait en C pur, plus rapide et plus stable — mémoire en attente dans la barre d'état réduite de plus de 95 % et taille du programme d'environ 98 %, choix des zones à nettoyer, vidage automatique du cache (anti-saccades en jeu), cache affiché sur l'écran d'accueil, réglages de nettoyage par défaut adaptés aux jeux et aux vidéos, bouton de retour aux valeurs par défaut, vérification des mises à jour et démarrage plus fiables |
| 2.0.3 | 2026-09-03 | Meilleure détection du plein écran pour ne pas interrompre jeux et vidéos, fermeture plus stable, notifications de fin plus exactes, nettoyages répétés optimisés, réglages plus stables |
| 2.0.2 | 2026-08-13 | Option pour sauter le nettoyage en plein écran, réglage de démarrage automatique retiré à la désinstallation, chargement des réglages et démarrage automatique plus fiables |
| 2.0.1 | 2026-07-13 | Nettoyage de la mémoire des navigateurs renforcé, meilleure stabilité sur de longues durées, notifications et réglages plus fiables, ajout de l'espagnol |

## Licence

MemoryCleaner est un **gratuiciel**. Vous pouvez l'utiliser gratuitement et sans restriction partout — au bureau, à la maison, dans les administrations ou à l'école — et le redistribuer librement.

## Liens

- Site web : <https://kilho.net/memorycleaner>
- Forum : <https://groups.google.com/g/kilhonet>
- X (Twitter) : <https://www.twitter.com/kilhonet>

© KILHO.NET
