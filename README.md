# Analyse des sols du Québec (2007-2024)

Dashboard interactif présentant l'évolution spatio-temporelle des indicateurs de fertilité des sols agricoles du Québec, basé sur plus de 600 000 analyses d'échantillons de sols.

## Aperçu

Ce tableau de bord permet de visualiser et comparer les données d'analyses de sols à l'échelle des régions administratives et des MRC du Québec sur la période 2007-2024.

### Indicateurs disponibles

- **Phosphore** (kg/ha) - Phosphore assimilable
- **Indice de saturation en phosphore (ISP)** (%) - Risque environnemental
- **pH eau** - Acidité du sol
- **Besoin en chaux** (t/ha) - Amendement calcique recommandé
- **Matière organique** (%) - Teneur en MO
- **Analyses >= 4% MO** (%) - Proportion atteignant le seuil du Plan d'agriculture durable

### Fonctionnalités

- Visualisation cartographique interactive (MapLibre GL + PMTiles)
- Basculement entre niveaux géographiques (Région / MRC)
- Choix de la statistique (Médiane / Moyenne)
- Filtrage par année ou vue globale
- Tableau de données triable et filtrable
- Export CSV des données
- Interface responsive (mobile/tablette/desktop)

## Technologies

- **Cartographie** : [MapLibre GL JS](https://maplibre.org/) + [PMTiles](https://protomaps.com/docs/pmtiles)
- **Fond de carte** : Carte du gouvernement du Québec
- **Données** : JSON optimisé (~1 Mo)
- **Hébergement** : GitHub Pages (statique, sans serveur)

## Fichiers

| Fichier | Description |
|---------|-------------|
| `index.html` | Application complète (HTML/CSS/JS) |
| `data.json` | Données agrégées par région/MRC et année |
| `mrc.pmtiles` | Tuiles vectorielles des MRC |
| `region.pmtiles` | Tuiles vectorielles des régions |

## Source des données

Les données proviennent de l'analyse d'échantillons de sols recueillis par des laboratoires privés entre 2007 et 2024. Elles ont été centralisées, nettoyées et agrégées par l'IRDA.

### Limites d'interprétation

- La géolocalisation repose sur les codes postaux (incertitude spatiale variable)
- Les pratiques d'échantillonnage ne sont pas aléatoires ni systématiques
- Certains échantillons peuvent provenir de milieux non agricoles

## Contact

- **Cédric Bouffard**, professionnel de recherche : cedric.bouffard@irda.qc.ca
- **Marc-Olivier Gasser**, chercheur : marc-o.gasser@irda.qc.ca

## Partenaires

<p align="center">
  <a href="https://www.quebec.ca/">
    <img src="https://www.foretouverte.gouv.qc.ca/particular/images/QUEB.png" alt="Gouvernement du Québec" height="50">
  </a>
  &nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://www.irda.qc.ca/">
    <img src="https://irda.qc.ca/dist/assets/logos/logo-irda-color.svg" alt="IRDA" height="40">
  </a>
</p>

## Licence

Ce projet est sous licence [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) (Attribution - Pas d'utilisation commerciale).

© IRDA - Institut de recherche et de développement en agroenvironnement
