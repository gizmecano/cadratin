# Cadratin

[English](README.md) | Français

## Introduction

Cadratin est un modèle [LibreOffice](https://www.libreoffice.org/) pour mettre en forme un manuscrit basé sur des [multiples du cadratin](https://fr.wikipedia.org/wiki/Cadratin) selon les normes typographiques françaises.

## Structure du fichier XML

Selon la [documentation officielle](https://help.libreoffice.org/latest/fr/text/shared/00/00000021.html?DbPAR=SHARED#bm_id3154408):

> Les documents au format OpenDocument sont stockés en tant qu'archives compressées contenant des fichiers XML. Pour afficher ces fichiers XML, vous pouvez ouvrir le fichier OpenDocument avec un programme de décompression. Les fichiers et répertoires suivants se trouvent dans les fichiers OpenDocument :

1. Le texte contenu dans le document se situe dans `content.xml`
2. Le fichier `meta.xml` contient les métadonnées du document, mais les valeurs mentionnant les paramètres d'impressions (`meta:printed-by` et `meta:print-date`) sont laissées vides
3. Le fichier `settings.xml` contient des informations complémentaires à propos du document en question, mais quelques valeurs mentionnant les paramètres d'impressions(`config:name="PrinterName"` et `config:name="PrinterSetup"`) sont laissées vides
4. les styles appliqués au document peuvent être trouvés dans le fichier `styles.xml`
5. Le fichier `META-INF/manifest.xml` décrit la structure du fichier XML

Des fichiers supplémentaires sont contenus dans le format de fichier compressé :

1. Le fichier `manifest.rdf` répertorie les fichiers présents dans le document et qui contiennent des métadonnées RDF, tels que `content.xml` et `styles.xml`
2. Le fichier `mimetype` contient le type de média MIME encodé en ASCII associé au document
