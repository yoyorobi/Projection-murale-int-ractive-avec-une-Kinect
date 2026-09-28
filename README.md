# Projection murale interactive : Spectre Néon

Une installation où le corps du visiteur devient un squelette de néon lumineux, projeté en temps réel sur un mur. Capté avec une Kinect v2 et programmé en nodal dans TouchDesigner.

## Contexte

Projet réalisé dans le cadre du cours de Médias interactifs (TP3, Techniques d'intégration multimédia, Cégep Édouard-Montpetit).

Le mandat : concevoir une expérience interactive combinant capture de mouvement et visuels en temps réel.

## Mon rôle

Projet solo : conception, direction visuelle, programmation nodale et page web de présentation.

## Technologies

- **TouchDesigner** : programmation nodale et rendu en temps réel
- **Kinect v2** : capture du squelette (jusqu'à deux joueurs)
- **HTML / CSS** : page de présentation du projet, en CSS seulement

## Fonctionnement

1. **Mode veille** : un système de cubes animés occupe l'écran tant que personne n'est détecté
2. **Détection** : dès qu'un joueur entre dans le champ, les cubes explosent vers l'extérieur
3. **Mode squelette** : chaque articulation devient un segment de néon coloré et lumineux
4. **Sabres laser** : chaque joueur tient un sabre attaché à son bras, avec vibration, détection du contact entre les deux sabres et détection des mouvements rapides pour déclencher les sons

## Démarche

1. **Idéation** : le squelette comme matière visuelle, en néon
2. **Squelette** : segments dessinés à partir des données de la Kinect, une couleur par segment
3. **Effet de lueur** : chaîne de flou, addition et ajustement de couleur pour l'aspect néon
4. **Mode veille et transition** : cubes animés qui explosent à l'arrivée d'un joueur
5. **Sabres laser** : direction du bras, détection de contact et de vitesse
6. **Page web** : présentation du projet avec une esthétique de grille de points en CSS

## Défi principal

**Problème :** faire réagir les sabres au bon moment, quand ils se touchent ou quand le joueur fait un mouvement rapide.

**Solution :** le contact est détecté par la distance entre les poignets des deux joueurs. Les mouvements rapides sont détectés par la vitesse du poignet, comparée à un seuil. Le tout avec des opérateurs, sans script.

## Installation et exécution

**Prérequis**
- Une Kinect v2 avec son adaptateur, branchée en USB 3.0
- Le SDK Kinect for Windows v2
- Windows

## Limites connues

- Nécessite une Kinect v2 et Windows
- Le SDK Kinect v2 peut poser des problèmes de compatibilité sur Windows 11
- Certains effets fluides (bruit animé par le temps) ralentissent les machines moins puissantes

## Crédits

- Conception, design et programmation : Yoan Robitaille
- Musique: https://pixabay.com/music/main-title-invasion-march-star-wars-style-cinematic-music-219585/

- Sound effects:
	Swoosh:
	https://pixabay.com/sound-effects/film-special-effects-lightsaber3-87667/
	Clash:
	https://www.101soundboards.com/sounds/25914-crash-1-lightsaber
	Humming:
	https://pixabay.com/sound-effects/film-special-effects-saber-hummingwav-14651/

- Tutoriel Autonome : https://www.youtube.com/watch?v=dwh5CS_0EDs

-Cards pour site web : https://uiverse.io/gharsh11032000/ancient-starfish-68

## Auteur

**Yoan Robitaille** · Dev média interactif / Dev web