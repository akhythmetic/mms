---
---
---

# ROUTINE ACP

## Analyse de données

### 1. Importer

``` r
data <- read.table(    , header=T, dec="   ")
```

### 2. Format structure de données  

```         
str()
as.factor()
```

### 3. Stat descriptive univariée 

```         
summary()
```

### 4. Stat descriptive bivariée [**quanti**]{.underline} 

-   correlation

-   nuage de points

-\> Matrice de corrélation sur les variables quanti

### 5. ACP sur les [quanti]{.underline}

``` r
quanti.sup=...
```

### 7. Analyse des Résultats de l'ACP

-   \% de variance expliquée par dimension + graphique

=\> Selection du nombre d'axes

-   Interpréter les axes (contribution des variables, p_valeurs)

-   Interpretation du nuage des individus
