---
title: "Gérer les permissions avec chmod"
date: 2026-06-11
author: Slim Ben Said
categories: [linux, débutant]
layout: single
---

Modifier les permissions des fichiers sous Linux.

## Comprendre les permissions

Chaque fichier a des droits pour propriétaire, groupe et autres.

## La commande chmod

```bash
chmod 755 script.sh    # exécutable par tous
chmod +x script.sh     # ajouter exécution propriétaire
chmod -w fichier.txt   # enlever écriture
```

## Notation symbolique

- `u` = propriétaire
- `g` = groupe
- `o` = autres
- `a` = tous

```bash
chmod u+x fichier
chmod g-w fichier
```

## Exercice

1. Créez `touch test.txt`
2. `chmod +x test.txt`
3. `ls -l test.txt`

Vous avez modifié les permissions !

