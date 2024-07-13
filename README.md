# Coin Afrique Scraper

Cette application Streamlit permet de télécharger des données extraites de Coin Afrique sur les "villas", "terrains" et "appartements".

## Fonctionnalités

- **Bibliothèques Python**: base64, pandas, streamlit
- **Source de données**: [Coin Afrique](https://sn.coinafrique.com/)
- **Options**:
  - Scraping des données avec BeautifulSoup
  - Téléchargement des données extraites
  - Tableau de bord des données
  - Remplissage du formulaire

## Prérequis

Avant de commencer, assurez-vous d'avoir installé les outils suivants :

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

## Installation

1. Clonez ce dépôt :
   ```sh
   git clone https://github.com/Mx-Bx/dit-devops-project.git
   cd dit-devops-project
   ```

2. Construisez l'image Docker :
   ```sh
   docker-compose build
   ```

3. Démarrez les services :
   ```sh
   docker-compose up
   ```

4. Accédez à l'application Streamlit dans votre navigateur à l'adresse suivante :
   ```
   http://localhost:8501
   ```

## Structure des fichiers

```plaintext
coin-afrique-scraper/
├── app.py          # Contient le code de l'application Streamlit
├── test_app.py     # Contient les tests unitaires pour l'application
├── Dockerfile      # Définit l'image Docker pour l'application
├── docker-compose.yml  # Définit les services Docker et leurs configurations
├── requirements.txt    # Liste des dépendances Python
├── README.md       # Fichier README principal du projet
└── data/
    ├── lien-1.csv
    ├── lien-2.csv
    ├── lien-3.csv
```

## Commandes pour exécuter les tests

Pour exécuter les tests unitaires, utilisez la commande suivante :
```sh
pytest
```

## Exemple d'utilisation

### Options

- **Scrape data using BeautifulSoup**:
  - Récupère les données à partir de Coin Afrique et les affiche dans un tableau.

- **Download scraped data**:
  - Télécharge les données extraites à partir des fichiers CSV locaux et les affiche dans un tableau.

- **Fill the form**:
  - Affiche un formulaire intégré à partir de KoboToolbox.

- **Dashboard of the data**:
  - Affiche un tableau de bord intégré à partir de Looker Studio.

## Aide

Si vous rencontrez des problèmes, n'hésitez pas à ouvrir une issue sur [GitHub](https://github.com/Mx-Bx/coin-afrique-scraper/issues).

## Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.
```