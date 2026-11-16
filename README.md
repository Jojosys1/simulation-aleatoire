# Simulation aléatoire

Travaux pratiques de **simulation en R** : génération de lois, moments, lois des
extrêmes, et tests statistiques (paramétriques et non paramétriques).

## Contenu

| Fichier / dossier | Rôle |
|---|---|
| `code_R_tests_param_et_non_param.Rmd` | Tests paramétriques et non paramétriques (Intima-Media, HTA) |
| `R_Simulation_code.qmd` | Code de simulation (Quarto) |
| `R_0_code_simulation.qmd` | Premier script de simulation (Quarto) |
| `rapports/` | Rapport de TP : `TP_SIMULATION.Rmd` (+ exports) et `TP_Devoir.Rmd` |
| `donnees/` | Jeux de données : `HTA.xlsx`, `Intima_Media.xlsx`, `nutriage.xlsx`, `TME_Afrique.xlsx` |
| `TP_Devoir.docx` | Énoncé / rendu du devoir |
| `Exemples_Moments_et_Lois des Extrêmes.docx` | Fiche d'exemples |
| `Exercices sur Tests Paramétriques et non Paramétriques_New.docx` | Feuille d'exercices |

## Prérequis

- **R** (≥ 4.2) avec `readxl`, `ggplot2`, `dplyr` (et `knitr` pour les rapports).
- **Quarto** pour rendre les `.qmd`.

```r
install.packages(c("readxl", "ggplot2", "dplyr", "knitr"))
```

## Utilisation

```bash
# Rendre le rapport principal
cd rapports && Rscript -e "rmarkdown::render('TP_SIMULATION.Rmd')"

# Rendre un script Quarto
quarto render R_Simulation_code.qmd
```

Les scripts chargent les données via `donnees/<fichier>.xlsx` (chemins relatifs au projet).

## Résultats

Les rapports rendus (`.html`, `.docx`, `.tex`) sont dans `rapports/`.
