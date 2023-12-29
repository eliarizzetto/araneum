---
title: "Notes on Git and GitHub"
enableToc: false
date: 2023-12-29 17:59
aliases:
- Git primer
- GitHub primer
place: Pordenone
tags:
- git
- github
---

## Comandi

Comando per rimuovere cartella (e tutti i file all'interno) dalla repository (e quindi dal tracking del version control), ma non dal file system locale:


$ git rm --cached -r <path/to/folder>

rm = remove
-r = --recursive, significa che toglie dalla repo anche i file e le altre cartelle all'interno della cartella

Questo comando funziona quando devi rimuovere una cartella che hai accidentalmente aggiunto al version control. Ad esempio, io l'ho utilizzato per togliere la cartella .idea di pycharm dalla repo: viene tolta sia dalla REPO locale (anche se è rimasta nel file system) sia, dopo commit and push, in quella remota.