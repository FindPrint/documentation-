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

## Auteur
Projet mené par **Zackary**.  

## Licence
MIT
