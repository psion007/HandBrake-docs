---
Type:            article
State:           [ draft ]
Title:           Chapitrage
Project:         HandBrake
Project_URL:     https://handbrake.fr/
Project_Version: 1.3.0
Language:        French
Language_Code:   fr
Authors:         [ Philip Sion (psion007) ]
Copyright:       2019 HandBrake Team
License:         Creative Commons Attribution-ShareAlike 4.0 International
License_Abbr:    CC BY-SA 4.0
License_URL:     https://handbrake.fr/docs/license.html
---

Chapitrage
==========

## Chapitres

HandBrake peut copier les marqueurs de chapitres à partir de votre source vers un fichier de sortie MP4, MKV ou WebM.

Sur HandBrake, si vous cliquez sur l'onglet "Chapters", vous verrez une liste des chapitres détectés. HandBrake générera automatiquement les noms de chapitre au format suivant : "Chapter n" avec n étant le numéro du chapitre.

![Chapters Tab](../../images/windows/chapters-1.0.0.png "Chapters Tab")

## Renommer les chapitres

Si vous le souhaitez, vous pouvez les renommer simplement en changeant les noms affichés dans l'onglet "Chapters".

Vous pouvez aussi importer ou exporter un ensemble de marqueurs de chapitre. HandBrake accepte l'importation de fichiers CSV (Comma Separated Values - Valeurs séparées par des point-virgules

Cliquez sur le bouton "Import" pour choisir un fichier CSV. Le fichier doit être au format suivant :

```
1,Nom du 1er chapitre
2,Nom du 2ème chapitre
3,Nom du 3ème chapitre
....
```

Vous pouvez aussi exporter la liste des chapitres en cours au format CSV en cliquant sur le bouton "Export".

## Sources sans chapitres

Malheureusement, HandBrake ne peut actuellement pas ajouter de marqueurs de chapitres s'ils n'existent pas déjà dans la source.
