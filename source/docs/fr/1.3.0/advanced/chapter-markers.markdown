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

## Renaming chapters

If you wish, you can rename these by simply simply altering the names shown in the chapters tab.

You can also import or export the set of chapter markers. HandBrake supports importing of CSV (Command seperated Values) files.

Click the Import button to choose a CSV file. The file must be in the following format:


```
1,Chapter Name
2,Chapter 2 Name
3,Chapter 3 Name
....
```

Finally, you can export the current chapter list to CSV format by clicking the 'export' button.

## Sources without chapters

Unfortunately, HandBrake can not currently add chapter markers if they did not already exist in the source.
