# Lab7 – Fonctions et Modularité

Application Python démontrant l'utilisation de fonctions modulaires pour l'analyse et le traitement de notes d'étudiants. Ce projet illustre les bonnes pratiques de programmation avec des fonctions réutilisables, paramétrables et documentées.

Le programme met en œuvre une architecture modulaire complète avec séparation des responsabilités, validation des données et génération de rapports personnalisables.

---

## Fonctionnalités

### Fonctions Statistiques
- **Moyenne** : calcul de la moyenne avec gestion des listes vides
- **Min/Max** : identification des notes minimale et maximale
- **Filtrage** : sélection des notes selon un seuil paramétrable

### Fonctions de Transformation
- **Normalisation** : conversion de notes depuis n'importe quel barème vers /20
- **Bonus automatique** : ajout d'un bonus paramétrable avec plafonnement à 20
- **Validation robuste** : gestion des cas limites et erreurs potentielles

### Génération de Rapports
- **Rapport personnalisable** : titre, seuil, bonus et barème configurables
- **Affichage formaté** : présentation claire des statistiques
- **Export fichier** : sauvegarde automatique en format texte
- **Synthèse complète** : notes originales, normalisées, avec bonus et statistiques

---

## Architecture
```
Lab7_fonctions.ipynb → Notebook Jupyter contenant :

1. Fonctions modulaires
   - moyenne() : calcul de moyenne avec protection liste vide
   - appliquer_bonus() : ajout de bonus avec plafonnement
   - filtrer_notes() : sélection selon seuil
   - min_max() : tuple (min, max) avec gestion cas vide
   - normaliser() : conversion vers barème /20
   - rapport() : génération complète du rapport

2. Programme principal
   - Données de test (notes sur 100)
   - Appel avec paramètres personnalisés
   - Affichage console du rapport
   - Export vers fichier texte

3. Sortie
   - rapport_notes.txt (encodage UTF-8)
```

---

## Installation

Cloner le projet :
```bash
git clone https://github.com/benhirtfatimaezzahra/Lab7.git
```

Ouvrir le notebook avec Jupyter :
```bash
cd Lab7
jupyter notebook Lab7_fonctions.ipynb
```

Ou utilisez JupyterLab :
```bash
jupyter lab Lab7_fonctions.ipynb
```

---

## Notes Techniques

### Concepts Python utilisés
- **Fonctions modulaires** : séparation claire des responsabilités
- **Docstrings** : documentation complète de chaque fonction
- **List comprehensions** : `[min(note + bonus, 20) for note in notes]`
- **Paramètres par défaut** : `bonus=1`, `seuil=12`, `sur=20`
- **Tuple unpacking** : `note_min, note_max = min_max(notes)`
- **f-strings** : formatage avec `:.2f` pour les décimales
- **Gestion de fichiers** : `with open()` et encodage UTF-8
- **Guard clauses** : `if not notes: return ...`
- **`if __name__ == "__main__":`** : bloc d'exécution conditionnel



## Démonstration



https://github.com/user-attachments/assets/59be26b8-22fb-4d75-b7d0-8f7b186228ca


---

## Auteur

**Nom :** Benhirt Fatima Ezzahra  
**Cours :** Introduction à Python  
**Date :** Novembre 2025  
**Encadré par :** Pr. Mohamed LACHGAR
