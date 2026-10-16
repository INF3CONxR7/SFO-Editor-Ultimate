# SFO Editor Ultimate

Éditeur de fichiers **PARAM.SFO** pour Windows : **PS3, PS4, PS Vita et PSP**. Ouvrez un `PARAM.SFO` pour voir tous ses paramètres, modifier leurs valeurs, leur type et leur longueur, ajouter des icônes PS3 au titre, puis enregistrer le fichier en toute sécurité.

**[Télécharger la dernière version](https://github.com/INF3CONxR7/SFO-Editor-Ultimate/releases/latest)** · [English](#english)

## Configuration requise

- Un PC sous Windows 64 bits (x64). Rien d'autre à installer : le runtime .NET est inclus dans l'exécutable.
- Aucune console n'est nécessaire : tout se fait sur les fichiers `PARAM.SFO` copiés sur le PC.
- Facultatif : l'application Discord ouverte sur le PC, pour l'activité Discord.

## Fonctionnalités

**Ouverture**

- `PARAM.SFO` par **Fichier > Ouvrir…**, **Ctrl+O**, glisser-déposer ou **double-clic sur un fichier `.sfo`** dans l'Explorateur.
- Plusieurs fichiers ouverts en même temps, chacun dans son onglet. Un fichier ouvert alors que l'application l'est déjà arrive dans un nouvel onglet de la même fenêtre.
- Fiche du fichier : titre du jeu, plateforme reconnue automatiquement (PS3, PS4, PS Vita, PSP), identifiant du titre et état du fichier.

**Paramètres**

- Tableau de tous les paramètres : nom, valeur, longueur et type, avec une description de chaque paramètre connu.
- Recherche (**Ctrl+F**), filtre par type ou sur les seuls paramètres modifiés, tri par colonne, affichage compact.
- Modification de la valeur, du type de donnée (chaîne de caractères, chaîne sans terminateur, entier 32 bits) et de la longueur maximale, avec la place utilisée en octets.
- Rétablir une valeur, rétablir toutes les valeurs, supprimer un paramètre, copier un nom ou une valeur.

**Icônes PS3**

- Fenêtre **Icônes PS3** (**Ctrl+I**) : boutons de manette, symboles du système et autres icônes de la PS3, avec recherche et catégories.
- Un clic copie l'icône (à coller avec **Ctrl+V**), un double-clic l'insère dans la valeur en cours de modification, par exemple dans le titre du jeu. Chaque icône occupe 3 octets.

**Enregistrement**

- **Enregistrer** (**Ctrl+S**) et **Enregistrer sous** (**Ctrl+Maj+S**).
- Le fichier est relu et contrôlé avant l'écriture, et une copie de sauvegarde (`.bak`) de l'original est conservée.

**Préférences**

- Thèmes **Nuit**, **Sombre** et **Clair**, interface en **français** et en **anglais**.
- Lancement au démarrage de Windows et ouverture des fichiers `.sfo` par double-clic (**Paramètres > Général**).
- **Activité Discord** : affiche le fichier en cours de modification sur votre profil Discord, avec un petit logo de la plateforme. Activée par défaut, désactivable dans **Paramètres > Discord**.

Raccourcis : **Ctrl+O** ouvrir · **Ctrl+S** enregistrer · **Ctrl+Maj+S** enregistrer sous · **F5** recharger · **Ctrl+W** fermer l'onglet · **Ctrl+Tab** onglet suivant · **Ctrl+F** rechercher · **Ctrl+I** icônes PS3 · **Suppr** supprimer le paramètre.

## Installation

1. Ouvrez la [dernière version](https://github.com/INF3CONxR7/SFO-Editor-Ultimate/releases/latest) et téléchargez **`SFOEditorUltimate-win-x64.zip`**. Le fichier `.zip.sig` sert au programme de mise à jour : inutile de le télécharger.
2. Extrayez l'archive à l'endroit de votre choix, par exemple dans Documents ou sur le Bureau : vous obtenez le dossier **`SFOEditorUltimate-win-x64`**. Gardez ensemble les deux fichiers qu'il contient : `SFO Editor Ultimate.exe` et `SFO Editor Ultimate Update.exe` (le programme de mise à jour).
3. Lancez **`SFO Editor Ultimate.exe`** depuis ce dossier.

> **Windows SmartScreen** : l'exécutable n'est pas signé Authenticode, Windows peut donc afficher « Windows a protégé votre ordinateur ». Cliquez sur **Informations complémentaires**, puis sur **Exécuter quand même**.

## Utilisation

1. Ouvrez un ou plusieurs `PARAM.SFO` (**Ctrl+O**, glisser-déposer sur la fenêtre ou double-clic dans l'Explorateur).
2. Sélectionnez un paramètre dans le tableau : il s'affiche à droite, dans **Édition du paramètre**.
3. Modifiez sa valeur (bouton **Icônes PS3** pour ajouter une icône), puis cliquez sur **Appliquer**.
4. Enregistrez avec **Ctrl+S**.

Bon à savoir : rien n'est écrit tant que vous n'enregistrez pas. Un onglet modifié est marqué, et l'application demande confirmation avant de fermer un fichier non enregistré.

## Limites

- L'application modifie des `PARAM.SFO` existants : elle ne crée pas de fichier vide et n'ajoute pas de nouveaux paramètres.
- Les icônes PS3 sont des caractères propres à la console : Windows ne sait pas les afficher, la fenêtre **Icônes PS3** en montre un aperçu approchant. Elles s'affichent normalement sur la PS3.
- L'application ne resigne rien : après avoir modifié le `PARAM.SFO` d'une sauvegarde PS3, mettez à jour son `PARAM.PFD` avec un outil de resignature.

## Mises à jour

Au démarrage, l'application vérifie sur GitHub si une nouvelle version est publiée. Si c'est le cas, **« Mise à jour X.Y.Z disponible »** apparaît dans la barre de titre : un clic, et l'application se ferme, installe la mise à jour, puis se relance. Vous pouvez aussi utiliser **Paramètres > Mises à jour > Vérifier les mises à jour**. Chaque version est **signée** : une version dont la signature est absente ou invalide est refusée. Aucun droit d'administrateur n'est demandé, sauf si l'application est installée dans un dossier protégé comme `C:\Program Files`.

`SFO Editor Ultimate Update.exe` peut aussi être lancé seul : il cherche la dernière version et l'installe si elle est plus récente.

## Désinstallation

1. Si vous les avez activés, désactivez d'abord le lancement au démarrage et l'ouverture des fichiers `.sfo` dans **Paramètres > Général**.
2. Supprimez le dossier de l'application.

Les préférences sont dans `%AppData%\SFO Editor Ultimate` et le journal des mises à jour dans `%LocalAppData%\SFO Editor Ultimate`.

## Support

- Discord : [discord.gg/TbFYvqsh5z](https://discord.gg/TbFYvqsh5z)
- Soutenir le projet : [ko-fi.com/INF3C7ONxR7](https://ko-fi.com/INF3C7ONxR7)

Développé par **INF3C7ONxR7**.

---

## English

**SFO Editor Ultimate** is a **PARAM.SFO** editor for Windows: **PS3, PS4, PS Vita and PSP**. Open a `PARAM.SFO` to see all its parameters, edit their values, type and length, add PS3 icons to the title, then save the file safely. The interface is available in French and English.

**Requirements**: Windows 64-bit (x64) PC, no .NET install needed · no console needed · optional: Discord app running for the Discord activity.

**Features**: open several `PARAM.SFO` files in tabs (menu, Ctrl+O, drag and drop or double-click a `.sfo` file in File Explorer) · file card with game title, detected platform (PS3, PS4, PS Vita, PSP) and title ID · parameter table with descriptions, search (Ctrl+F), type filter, sorting and compact view · edit value, data type and maximum length, with the bytes used · restore one or all values, delete a parameter, copy a name or value · **PS3 icons** window (Ctrl+I): click to copy, double-click to insert controller buttons and system symbols into a value · Save (Ctrl+S) and Save as (Ctrl+Shift+S), with a check before writing and a `.bak` backup of the original · Nuit, Sombre and Clair themes · start with Windows and `.sfo` file association (Settings > General) · Discord activity with a platform badge (on by default, can be turned off).

**Install**: download **`SFOEditorUltimate-win-x64.zip`** from the [latest release](https://github.com/INF3CONxR7/SFO-Editor-Ultimate/releases/latest) (not the `.sig` file, which is used by the updater), extract it wherever you like to get the **`SFOEditorUltimate-win-x64`** folder, keep both files together and run **`SFO Editor Ultimate.exe`**. The executable is not Authenticode-signed, so Windows SmartScreen may show "Windows protected your PC": click **More info**, then **Run anyway**.

**Limits**: edits existing `PARAM.SFO` files only (no blank file, no new parameters) · PS3 icons are console characters that Windows cannot display (approximate previews in the app) · nothing is resigned: after editing a PS3 save's `PARAM.SFO`, update its `PARAM.PFD` with a resigning tool.

**Updates**: the app checks GitHub at startup; when a new version is out, click **"Update X.Y.Z available"** in the title bar (or **Settings > Updates > Check for updates**). Every release is signed; unsigned or tampered releases are refused.

**Uninstall**: turn off startup and `.sfo` file association in **Settings > General** if you enabled them, then delete the app folder. Settings are in `%AppData%\SFO Editor Ultimate`, the update log in `%LocalAppData%\SFO Editor Ultimate`.

**Support**: [Discord](https://discord.gg/TbFYvqsh5z) · [Ko-fi](https://ko-fi.com/INF3C7ONxR7) · Developed by **INF3C7ONxR7**.
