# Classification de texte par méthodes NLP

Ce projet vise à prédire si une personne est chef de ménage ou non en utilisant des données de recensement, en se basant sur plusieurs méthodes de traitement et d'analyse.

## Description du Projet
Dans ce projet, nous avons exploré plusieurs approches pour prédire si une personne est chef de ménage en utilisant des techniques de Machine Learning pour le Traitement du Langage Naturel (NLP). Les principales méthodes utilisées sont les arbres de classification par gradient boosting, les modèles Transformer Encoder-Decoder, et le fine-tuning d'un modèle pré-entrainé BERT.

## Contenu du Répertoire
Tout le code utilisé pour l'analyse se trouve dans le répertoire `src`. <br>
Le noteook `src/eda.ipynb` contient le code pour l'analyse exploratoire des données, et le notebook `src/modelling.ipynb` contient le code où sont implémentés et entrainés les différents modèles.

## Dépendances
Assurez-vous que toutes les dépendances sont installées en utilisant la commande `pip install -r requirements.txt`.
 
## Différentes approches
### Gradient Boosting
Nous avons initialement utilisé des arbres de classification par gradient boosting pour analyser les données tabulaires du recensement. Le modèle a été entraîné en utilisant un encodage simple des données et une grid search exhaustive pour optimiser les hyperparamètres. Les résultats étaient prometteurs mais semblaient pouvoir être améliorés.

### Transformers Encoder-Decoder
Nous avons ensuite exploré l'utilisation de modèles Transformer Encoder-Decoder, en particulier le réseau BART, pour encoder les données de manière plus intelligente. Cependant, les résultats n'ont pas été aussi prometteurs que prévu en raison de la perte de la structure tabulaire des données.

### Fine-tuning avec BERT
Enfin, nous avons réalisé un fine-tuning d'un modèle pré-entrainé adapté de BERT pour obtenir des performances élevées sans overfitting. Cette approche a donné les meilleurs résultats en termes de performance.

## Licence

Ce projet est sous licence MIT - voir le fichier [LICENSE.md](LICENSE.md) pour plus de détails.