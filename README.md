# dagcc (Docker Asm GCC)

La base docker pour un projet en assembleur.

<details>
  <summary>Table des matières</summary>
  <ol>
    <li>
        <a href="#création-du-conteneur-docker">Création du conteneur (Docker)</a>
        <ul>
            <li><a href="#le-fichier-env">Le fichier .env</a></li>
            <li><a href="#installer-le-conteneur">Installer le conteneur</a></li>
        </ul>
    </li>
    <li><a href="#rechercher-un-package-docker">Rechercher un package (Docker)</a></li>
    <li><a href="#install-un-package-docker">Install un package (Docker)</a></li>
    <li><a href="#le-dossier-du-projet">Le dossier du projet</a></li>
    <li><a href="#compile">Compile</a></li>
    <li><a href="#disassemble">Disassemble</a></li>
  </ol>
</details>

## Création du conteneur (Docker)
Vous devez avoir installé Docker.
Pour la création du conteneur docker pour le projet.
### Le fichier .env
Modifier le fichier .env :
```
NAME_GCC_CONTAINER=dagcc_gcc
```
Par le nom de votre projet, par exemple 'tintin' :
```
NAME_GCC_CONTAINER=tintin_gcc
```


### Installer le conteneur
Vous pouvez créer votre projet.
```
$ ./install.sh
```

## Le dossier du projet
Votre code devra être placé dans le dossier "**project**"

## Rechercher un package (Docker)
Si vous avez besoin d'un package pour votre projet dans le conteneur. Vous pouvez rechercher les packages disponibles pour le conteneur.
```
$ ./bin/terminal.sh
# apt-cache search gcc
```

## Install un package (Docker)
Si vous avez besoin d'installer un package dans votre conteneur.
```
$ ./bin/terminal.sh
# apt install gcc
```
