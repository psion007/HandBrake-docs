---
Type:            article
State:           [ draft ]
Title:           Audio and Subtitle Defaults
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

Réglages par défaut pour l'audio et les sous-titres
===================================================

HandBrake ne stocke pas les réglages de l'audio et des sous-titres dans les préréglages.

A la place, nous stockons des règles comportementales pour sélectionner automatiquement l'audio et les sous-titres à chaque fois que vous scannez une nouvelle source ou sélectionnez un titre.

Pour configurer le comportement de la sélection de piste, cliquez sur le bouton "Configure Defaults" dans l'onglet Audio ou Subtitle.

### Réglages audio par défaut

![Audio Defaults Window](../../images/windows/audio-defaults-1.0.0.png "Audio Defaults Window")

- Track Selection Behaviour
  - None
    - Aucune piste audio ne sera ajoutée automatiquement.
  - First matching selected Language
    - Ajoute la première piste qui fait partie de la liste des "Chosen Languages", ou sinon la première piste sera sélectionnée.
  - All matching selected languages
    - Ajoute toutes les pistes qui font partie de la liste des "Chosen Languages".
- Choose Languages
  - Déplace les langues qui vous intéressent dans la liste des "Chosen Languages" afin de pouvoir sélectionner automatiquement les pistes à l'aide de la sélection de piste comportementale.
- Auto Passthru
  - HandBrake peut préserver plusieurs formats audio (pass-through). Il y a différentes options dans le sélecteur de l'encodeur audio pour cela. Lorsque vous sélectionnez "Auto Passthru", il recopiera sans modifications tous les formats supportés. Vous pouvez limiter ce qu'il recopiera automatiquement. Par exemple, si vous souhaitez seulement conserver l'AC3 et le DTS "tel quel", mais aucun des autres choix, décochez les cases à cocher correspondantes.
  
- Fallback Encoder
  - Lorsque vous avez sélectionné un encodage sans modification mais que le format de la piste ne correspond pas à ce format, HandBrake réencodera automatiquement la piste. L'encodeur "de rechange" (fallback encoder) est l'encodeur sur lequel HandBrake basculera par défaut.
  
### Sous-titres par défaut

![Subtitle Defaults Window](../../images/windows/subtitle-defaults-1.0.0.png "Subtitle Defaults Window")

- Track Selection Behaviour
  - None
    - Aucune piste de sous-titres ne sera ajoutée
  - First matching selected Language
    - Ajoute la première piste de sous-titres qui appartient à la liste des "Chosen Languages", lorsque cela est supporté par le conteneur de sortie. 
  - All matching selected languages
    - Ajoute toutes les pistes de sous-titres qui font partie de la liste des "Chosen Languages", lorsque cela est supporté par le conteneur de sortie. 
- Burn in Behaviour
  HandBrake peut graver une piste de sous-titres sur un fichier pendant l'encodage. Il y a 3 types de comportements que vous pouvez choisir pour cette casse à cocher pour être sélectionnée automatiquement.
  - Foreign Audio Scan : Recherche audio en langue étrangère
  - First Track : Première piste
  - Foreign Audio Preferred, else first : Recherche audio en langue étrangère, sinon première piste
- Choose Languages
  - Déplace les langues qui vous intéressent dans la liste des "Chosen Languages" afin de pouvoir sélectionner automatiquement les pistes à l'aide de la sélection de piste comportementale.
- Add Closed Captions when available
  - Les "Close captions" sont des sous-titres au format texte supportés par les fichiers MP4 et MKV. Si vous sélectionnez cette option, HandBrake les copiera automatiquement dans le fichier de sortie.
- Add Foreign Audio Scan
  - HandBrake réalisera un scan du titre / du fichier source pour essayer de détecter s'ils y a des portions du titres qui sont dans une langue étrangère. S'il en détecte une, il ajoutera la piste de sous-titres automatiquement. 
