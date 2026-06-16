English is following.  

# Avertissement  
## Statut du projet et limitation de responsabilité  
Ce dépôt contient du code, des données et de la documentation qui sont toujours en cours de développement. Le contenu est fourni "tel quel", sans aucune garantie d’aucune sorte, expresse ou implicite, y compris, sans s’y limiter, les garanties de qualité marchande, d’adéquation à un usage particulier ou d’absence d’erreurs.
Les auteurs et contributeurs de ce dépôt ne garantissent pas l’exactitude, l’exhaustivité, la fiabilité ou la pertinence du contenu pour un quelconque usage.
Toute utilisation du contenu de ce dépôt se fait aux seuls risques et périls de l’utilisateur.
En aucun cas, les auteurs, contributeurs ou organisations associées à ce dépôt ne pourront être tenus responsables de dommages directs ou indirects, pertes de données, pertes financières ou de toute autre conséquence résultant de l’utilisation, de la modification ou de la redistribution du contenu par des tiers.
  
# Modèles  
Ce dépôt vise à documenter les modèles développés dans le cadre de l'initiative [Archétype QC](https://github.com/Archetype-QC). Les modèles déposés dans ce dépôt sont organisés selon la structure suivante:  
- [Prototypes-Batiments-Buildings](https://github.com/Archetype-QC/Modeles-Models/tree/main/Prototypes-Batiments-Buildings): ce dossier regroupe les prototypes de bâtiments actuellement disponibles dans le dépôt (résidentiel et commercial-institutionnel), ainsi que deux fichiers CSV de synthèse:
  - `Liste-Modeles-Batiments.csv` (version française);
  - `List-Building-Models.csv` (version anglaise, mêmes modèles).
  - Le répertoire [R](https://github.com/Archetype-QC/Modeles-Models/tree/main/Prototypes-Batiments-Buildings/R) contient les modèles du secteur résidentiel et inclut les sous-répertoires suivants;
    - `MU` (Multi-Unit) pour les immeubles à logements multiples incluant `Apt` (les immeubles à appartements de moyenne [MR] et haute [HR] hauteur), `Dup` (duplex) et `Trip` (triplex);
    - `SF` (Single-Family) pour les logements unifamiliaux incluant `Det` (maisons détachées), `Row` (maisons en rangée) et `SD` (les maisons semi-détachées ou jumelées).
  - Le répertoire [CI](https://github.com/Archetype-QC/Modeles-Models/tree/main/Prototypes-Batiments-Buildings/CI) contient les modèles du secteur commercial-institutionnel, et plus spécialement les sous-répertoires suivants:
    - `EDU` pour le secteur de l'éducation avec des modèles d'écoles.
  - Le contenu type d'un dossier de modèle inclut le fichier `.osm` du modèle OpenStudio, le fichier EnergyPlus `in.idf` équivalent au fichier `.osm`, le rapport de simulation EnergyPlus `eplustbl.htm` et deux fiches descriptives PDF (`Fiche energie.pdf` pour la version française, `Energy card.pdf` pour la version anglaise).

Explication de l'arborescence du dépôt:
```text
Modeles-Models/                     Racine du dépôt
|-- README.md                       Présentation générale du dépôt en français et en anglais
|-- LICENSE-FR                      Licence du dépôt en français
|-- LICENSE-EN                      Licence du dépôt en anglais
\-- Prototypes-Batiments-Buildings/ Prototypes de bâtiments et fichiers CSV de synthèse
  |-- Liste-Modeles-Batiments.csv  Liste des modèles avec colonnes en français
  |-- List-Building-Models.csv     Liste des mêmes modèles avec colonnes en anglais
  |-- R/                           Modèles du secteur résidentiel
  |   |-- MU/                      Bâtiments résidentiels multi-logements
  |   |   |-- Apt/                 Immeubles à appartements
  |   |   |   |-- HR/              Modèles d'immeubles à appartements de grande hauteur
  |   |   |   \-- MR/              Modèles d'immeubles à appartements de moyenne hauteur
  |   |   |-- Dup/                 Modèles de duplex
  |   |   \-- Trip/                Modèles de triplex
  |   \-- SF/                      Bâtiments résidentiels unifamiliaux
  |       |-- Det/                 Modèles de maisons détachées
  |       |-- Row/                 Modèles de maisons en rangée
  |       \-- SD/                  Modèles de maisons semi-détachées ou jumelées
  \-- CI/                          Modèles du secteur commercial et institutionnel
    \-- EDU/                     Modèles du secteur de l'éducation, notamment des écoles
```

Note sur la convention de nommage des modèles: les acronymes dans les noms et chemins indiquent le secteur, le type de bâtiment, la configuration (ex. `Att` pour attaché et `Det` pour détaché) et la période de construction (ex. `pre1945`, `1946-1970`, `post2012`).  
  
--------------------------------------------------------------------------------
# Disclaimer  
## Project Status and Limitation of Liability  
This repository contains code, data, and documentation that is under active development. The content is provided "as is", without warranty of any kind, express or implied, including but not limited to warranties of merchantability, fitness for a particular purpose, or absence of defects.
The authors and contributors of this repository make no guarantees regarding the accuracy, completeness, reliability, or suitability of the content for any specific use.
Any use of the content is made entirely at the user’s own risk.
Under no circumstances shall the authors, contributors, or any affiliated organizations be held liable for any direct or indirect damages, data loss, financial loss, or any other consequences arising from the use, modification, or redistribution of the content by third parties.
  
# Models
The purpose of this repository is to document the models developed in the initiative [Archetype QC](https://github.com/Archetype-QC). The models available in this repository are organized according to the following structure:  
- [Prototypes-Batiments-Buildings](https://github.com/Archetype-QC/Modeles-Models/tree/main/Prototypes-Batiments-Buildings): this folder gathers the building prototypes currently available in the repository, covering both residential and commercial-institutional sectors, as well as two summary CSV files:
  - `Liste-Modeles-Batiments.csv` (French version);
  - `List-Building-Models.csv` (English version, listing the same models).
  - The [R](https://github.com/Archetype-QC/Modeles-Models/tree/main/Prototypes-Batiments-Buildings/R) directory contains models from the residential sector and includes the following subdirectories;
    - `MU` (Multi-Unit) for multi-unit residential buildings, including `Apt` (apartment buildings of medium [MR] and high [HR] rise), `Dup` (duplexes), and `Trip` (triplexes);
    - `SF` (Single-Family) for single-family dwellings, including `Det` (detached houses), `Row` (row houses), and `SD` (semi-detached houses).
  - The [CI](https://github.com/Archetype-QC/Modeles-Models/tree/main/Prototypes-Batiments-Buildings/CI) directory contains models from the commercial-institutional sector, and more specifically the following subdirectories:
    - `EDU` for the education sector, with school models.
  - The typical content of a model folder includes the `.osm` OpenStudio model file, the EnergyPlus `in.idf` file corresponding to the `.osm` file, the EnergyPlus simulation report `eplustbl.htm`, and two descriptive PDF sheets (`Fiche energie.pdf` for the French version and `Energy card.pdf` for the English version).

Explanation of the repository tree:
```text
Modeles-Models/                     Repository root
|-- README.md                       General repository overview in French and English
|-- LICENSE-FR                      Repository license in French
|-- LICENSE-EN                      Repository license in English
\-- Prototypes-Batiments-Buildings/ Building prototypes and summary CSV files
    |-- Liste-Modeles-Batiments.csv  List of models with French column headers
    |-- List-Building-Models.csv     List of the same models with English column headers
    |-- R/                           Residential sector models
    |   |-- MU/                      Multi-unit residential buildings
    |   |   |-- Apt/                 Apartment buildings
    |   |   |   |-- HR/              High-rise apartment building models
    |   |   |   \-- MR/              Mid-rise apartment building models
    |   |   |-- Dup/                 Duplex models
    |   |   \-- Trip/                Triplex models
    |   \-- SF/                      Single-family residential buildings
    |       |-- Det/                 Detached house models
    |       |-- Row/                 Row house models
    |       \-- SD/                  Semi-detached house models
    \-- CI/                          Commercial and institutional sector models
        \-- EDU/                     Education sector models, notably schools
```

Note on the model naming convention: the acronyms used in file and directory names indicate the sector, building type, configuration (for example `Att` for attached and `Det` for detached), and construction period (for example `pre1945`, `1946-1970`, `post2012`).
