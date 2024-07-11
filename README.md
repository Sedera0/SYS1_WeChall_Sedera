# WeChall
Warchall Challenge

## Enregistrement

- Inscription sur WeChall :
    ```bash
    ssh -p 19198 sedera@warchall.net
    ```
   Saisie dans le terminal avec mot de passe.

## Level 0

- Affichage des répertoires avec `cat WELCOME.md` :
    - `/home/level`
    - `/home/user/yournick/level`

- Exploration du premier répertoire avec `cd` et listing avec `ls`.

- Entrée dans "00_Welcome" avec `cd`, listing avec `ls`, et lecture de la solution avec `cat README.md`.

## Level 1

- Recherche de la solution dans "01_choice_tree" manuellement ou avec :
    ```bash
    grep -rn "solution" *
    ```
   Affichage direct de la solution.

## Level 2

- Accès à "02" avec `ls -al` pour les fichiers cachés, puis entrée dans ".porb" avec `cd .porb` et affichage avec `ls -al`.

- Obtention de la solution avec `cat .solution`.

## Level 3

- Entrée dans "03" avec `ls -al` pour les fichiers cachés, puis récupération de la solution avec `cat .bash_history`.

## Level 4

- Ouverture de "README.nfo" dans "04_kwisatz", suivi de l'indication "Look in your ~".

- Retour dans le répertoire avec `cd /level/04_kwisatz`, vérification des permissions avec `ls -l`, et modification avec :
    ```bash
    chmod 700 README.md
    ```
   Ouverture du fichier pour obtenir la solution.

## Level 5

- Il suffit d'entrer dans "05_privacy" avec `cd` puis `ls` et de faire la commande
    ```bash
    cat README.md
    ```
- Et on a la solution

## Level 10

- Pour le "Choose Your Path", entrer dans le dossier avec `cd` pui `ls`.

- Copier le contenu du dossier contenant la solution dans le répertoire personnel avec la commande :
    ```bash
    ./charp "so & cat solution.txt > ~/s.txt"
    ```
   (s.txt est le nom donné au fichier texte).

- Aller dans le répertoire personnel et afficher avec `cat s.txt`.

## Level 12

- Pour le level "Py-Tong", entrer dans le dossier avec `cd` puis faire `ls`.

- Exécuter le script Python avec la commande :
    ```bash
    ./pytong <(echo aaa)
    ```
   (echo aaa crée un fichier temporaire qui affiche la sortie de la commande).

- Obtenir la solution à côté de "return".

## Level 14

- Accéder à [https://www.wechall.net/challenge/warchall/live_lfi/index.php](https://www.wechall.net/challenge/warchall/live_lfi/index.php).

- Cliquer sur "Live LFI", suivi de la redirection.

- Changer le langage en PHP, puis décoder le texte avec :
    ```bash
    echo "text encoder" | base64 -d
    ```

- Obtenir la solution après le retour.

## Level 15

- Pour le niveau 15, procéder de manière similaire au niveau 14, mais changer le langage en "data".

- Examiner le code source du site pour trouver la solution sous "NOTHING HERE!!" en faisant défiler vers le bas.
