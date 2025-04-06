
# 🔬 Projet Bioinformatique – Analyse comparative du gène COX1

## 🧠 Objectif
Ce projet a pour but de récupérer, aligner et analyser le gène **COX1 (Cytochrome c Oxidase subunit I)** de plusieurs espèces à l’aide de **Biopython** et d’outils bioinformatiques en ligne comme **Clustal Omega** et **BLAST**.

## 🧰 Outils utilisés

- Python 3
- [Biopython](https://biopython.org/)
- [Clustal Omega (API REST – EMBL-EBI)](https://www.ebi.ac.uk/Tools/msa/clustalo/)
- [BLAST (NCBI)](https://blast.ncbi.nlm.nih.gov/)

## 📁 Structure du projet

```
.
├── data/
│   ├── sequences/
│   │   ├── Homo_sapiens_COX1.fasta
│   │   ├── Pan_troglodytes_COX1.fasta
│   │   ├── Gallus_gallus_COX1.fasta
│   │   ├── COX1_combined.fasta
│   │   └── COX1_aligned.fasta
│   └── XML/
│       └── blast_result.xml
├── main.ipynb
└── README.md
```

## 🔄 Étapes du projet

### 1. 📥 Téléchargement des séquences COX1
Utilisation de l'API **Entrez** (NCBI) via Biopython pour récupérer les séquences du gène COX1 pour :
- *Homo sapiens*
- *Pan troglodytes*
- *Gallus gallus*

---

### 2. 🧬 Fusion des séquences FASTA
Les séquences individuelles sont rassemblées dans un fichier FASTA unique (`COX1_combined.fasta`) pour l’alignement.

---

### 3. 🔗 Alignement multiple via Clustal Omega
Utilisation de l’**API web Clustal Omega (EMBL-EBI)** pour effectuer un alignement multiple des séquences ADN.

---

### 4. 👁️ Visualisation de l’alignement
Chargement et affichage des premières positions de l’alignement pour vérifier la qualité de l’alignement.

---

### 5. 🚀 Analyse BLAST
Lancement d’un **BLASTN** sur la séquence COX1 humaine pour rechercher des homologues dans la base de données `nt` de NCBI.  
Les 3 premiers résultats sont affichés avec leur score, pourcentage d'identité et alignement partiel.

---

## 📌 Résultat attendu
- Un alignement multiple des gènes COX1 montrant les régions conservées entre espèces.
- Une première vue des relations évolutives possibles.
- Des alignements BLAST indiquant des similarités avec d’autres séquences dans la base de données.

## 📧 Contact
**Auteur** : Abdoul Wahab Soumaré  
**Mail** : abdoulwahab.soumare@ucad.edu.sn
