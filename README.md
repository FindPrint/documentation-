# Validation d’un modèle stochastique avec mémoire et dimension effective dynamique

## Contexte
Ce projet explore un modèle inspiré de Ginzburg–Landau, enrichi par un terme de mémoire et une dimension effective dynamique.  
Il est validé sur données **synthétiques** puis appliqué à des données **réelles PM2.5 (Beijing, 2010–2014)**.

## Méthodologie
- Simulation synthétique avec balayage de paramètres.  
- Analyse réelle sur données PM2.5.  
- Estimation de α_mean par plusieurs méthodes (statistique, log, spectre).  
- Calibration automatique du facteur d’échelle.  

## Résultats
- **Synthétique** : erreurs < 0.1 %, robustesse confirmée.  
- **Réel** : calibration réussie, erreur finale < 10 %.  
- Rapports exportés dans `documentation/` et `resultats/`.  

## Structure du dépôt
- `documentation/` → README.txt, journaux, rapports.  
- `resultats/` → exports automatiques (rapports, figures).  
- `notebooks/` → notebooks Colab/Jupyter.
- ## Comment exécuter

### Option 1 — Google Colab
1. Ouvrir [Google Colab](https://colab.research.google.com/).
2. Importer le notebook depuis le dossier `notebooks/` (ex. `analyse_pm25.ipynb`).
3. Vérifier que le fichier de données (`donnees_reelles_clean.csv`) est présent dans l’environnement.
4. Exécuter les cellules dans l’ordre :
   - Phase synthétique (simulation, robustesse, rapport final).
   - Phase réelle (nettoyage, estimation de α_mean, calibration, rapport final).

### Option 2 — Local (Python ≥ 3.9)
1. Cloner le dépôt :
   ```bash
   git clone https://github.com/FindPrint/documentation-.git
   cd documentation-
   pip install -r requirements.txt
   jupyter notebook
   

## Auteur
Projet mené par **Zackary**.  

## Licence
MIT
