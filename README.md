# Modded sur Mac!

Oui vous avez bien entendu, après de longues heures de debugging j'ai trouvé une technique qui marche assez bien.

## Le launcher

Comme launcher nous allons utiliser [PrismLauncher](https://prismlauncher.org). C'est la même chose que PolyMC mais en plus sûr (PolyMC a été backdoor par un des devs, d'ailleurs je vous conseille de le désinstaller). Nous l'utilisons car le launcher est très utile pour configurer son jeu.

Allez sur https://prismlauncher.org et téléchargez la version Universal

![CleanShot 2022-12-10 at 10 18 39@2x](https://user-images.githubusercontent.com/74014262/206842963-187c42eb-6bed-486f-a4ad-909d72aa86c7.png)

## La version de java

Pour faire tourner modded, nous avons besoin d'une version de java en architecture x86 64-bit (la version .dmg).
Vous pouvez trouver java 16 ici: https://www.azul.com/downloads/?version=java-16-sts&os=macos&package=jdk&show-old-builds=true

![CleanShot 2022-12-10 at 10 23 55](https://user-images.githubusercontent.com/74014262/206843206-f9f784c8-5f56-4eed-bc89-eac8e4b3a9da.gif)

**Faites attention à ne pas prendre la mauvaise version!**

Une fois téléchargé, ouvrez le .dmg et suivez les instructions d'installation. Si une pop-up vous dit que java 16 x86 64-bit n'est pas compatible avec votre appareil, ignorez la.

## Télécharger Modded

Pour télécharger Modded, vous pouvez aller sur https://paladium-pvp.fr et télécharger le launcher (Modded.fr ne donne pas de lien de téléchargement, mais paladium si).

Une fois téléchargé, ouvrez le launcher (paladium-group) et installez Modded dans sa section. Nous avons besoin de faire ça pour générer les bons fichiers.

**Ensuite appuyer sur Jouer et les fichiers de téléchargeront. (modded ne se lancera pas)**

Une fois les fichiers téléchargés, vous pouvez quitter __paladium_group__

## Télécharger le patch jcef

Modded utilise une librairie nommée jcef. Mais celle ci en soit est incompatible avec mac. C'est pour ça que nous devons télécharger une version patch.
Pour télécharger le patch, aller sur https://drive.google.com/file/d/1aDeoBLTdpe3LKjuEtStmGbMWQIPl6fXY/view?usp=sharing (il a été compilé par moi, c'est pour ça qu'il est sur google drive)

## Configurer PrismLauncher

Maintenant que tout les fichiers sont téléchargés, nous pouvons aller créer une instance dans PrismLauncher.
Pour se faire, ouvrez PrismLauncher, selectionnez votre langue et ensuite, comme version java, selectionnez la **16.0.2 x86 64-bit**.

<img width="607" alt="Capture d’écran 2022-12-10 à 10 46 51" src="https://user-images.githubusercontent.com/74014262/206845936-817a9cbf-ef26-4c13-8f06-9ef984454597.png">

Une fois cela fait, appuyer sur le bouton "Finit" tout en bas à droite (en bleu). Sur la page principal, appuyer sur le bouton "Comptes" tout en haut à droite, et selectionnez "Configurer les comptes"

Une fois que la nouvelle fenêtre s'ouvre, cliquez sur le bouton tout en haut à droite "Ajouter un compte microsoft" et connectez votre compte.

## Enfin! Créer son instance Modded

Une fois tout cela fait, nous pouvons maintenant créer une instance minecraft pour jouer à Modded!
Fermez toute les fenêtre à part la page principal. Sur la page principal, cliquez sur "Ajouter une Instance". Vous devez selectionner la version **1.16.5** et comme **Chargeur de Mod, Forge (et pour la version selectionnez celle avec la petite étoile)**. Vous pouvez aussi donner un nom à votre instance.

Une fois l'instance crée, allez sur la page principal et en selectionnant l'instance, appuyer sur "Modifier"

Là, allez dans la section "Paramètres" et activez "Installation Java", "Arguments Java" et "Mémoire"

Dans Installation Java, activez "Passer les vérifications de compatibilité de Java" et verifiez que la version selectionnée est bien java 16 (par défaut, c'est le cas)

Dans Mémoire, augmentez `Allocation minimale de la mémoire` à `2048`, et `Allocation minimale de la mémoire` à `4480`. (C'est nécéssaire pour lancer modded)

Dans Arguments Java, collez `-Dfml.earlyprogresswindow=false` dans la boite de texte.

## Copier les fichiers Modded

Pour copier les fichiers modded dans votre instance, cliquez sur finder dans la barre des applications. Puis, glissez votre souris vers le haut de l'écran pour que la barre d'options aparaisse. Sur la barre, appuyer sur "Aller", puis appuyez sur "Aller au dossier" tout en bas.

Ensuite, collez `/Users/<utilisateur>/Library/Application Support/.modded` dans la boite de texte ou `<utilisateur>` est votre chemin d'utilisateur (il écrit dans la bar latéral à gauche de finder, son icone c'est une maison).

Vous aurez un dossier `.modded` qui va apparaître. Dans le dossier, selectionnez tout les fichiers/dossiers, et copiez les.

**Finalement, aller dans la page de configuration de votre instance** et dans l'onglet version, appuyer sur le bouton **"Ouvrir .minecraft"** à droite (4eme bouton en partant du bas)

Une fois dans le dossier, collez tout les fichiers modded. **Si des fichiers existent déjà sous le même nom, remplacez les.**

## Appliquer le patch

Si vous essayer de lancer modded, minecraft va crash. Pour régler cela, dezipez le fichiers jcef.zip que vous avez téléchargé avant.
Ensuite, copier le dossier jcef et collez le dans dossier `externalLibraries` qui se trouve dans `.minecraft`

# Profitez!

Oui c'était long mais ça vaut la peine! Vous pouvez maintenant jouer à Modded!

En cas de crash, ou de bug, contactez **Origaming#0001** sur discord. **ATTENTION** si trop de personne me dm, je risque de les bloquer. Donc envoyez moi un message seulement si vous arrivez vraiment pas.
