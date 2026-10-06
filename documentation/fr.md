<!-- ELUCENIA technical documentation · has-bled · fr · no clinical/professional/rights approval -->

# HAS-BLED

[conditions, sources et autorisations](https://elucenia.org/fr/outils/has-bled)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Hypertension non contrôlée (pression artérielle systolique \> 160 mmHg)

`h`

### Fonction rénale altérée (dialyse, greffe ou créatinine ≥ 2,26 mg/dL)

`rim`

### Fonction hépatique altérée (cirrhose ou bilirubine \> 2× et ASAT/ALAT \> 3× la normale)

`fig`

### AVC antérieur

`avc`

### Antécédent hémorragique ou prédisposition (anémie, thrombopénie)

`sang`

### INR instable (temps dans la cible thérapeutique \< 60 %)

`inr`

### Âge \> 65 ans

`idoso`

### Antiagrégant ou anti-inflammatoire

`drogas`

### Alcool (≥ 8 verres par semaine)

`alcool`

## Édition de la méthode

HAS-BLED/Pisters 2010 : 9 points ; rein/foie/médicaments/alcool séparés ; contexte ESC 2024

## Formule documentée

Un point par item : H hypertension, A anomalie rénale/hépatique (1 chacune), S AVC, B saignement, L INR labile, E âge (\> 65), D médicaments/alcool (1 chacun). Maximum : 9.

## Limites et population

Le HAS-BLED original estime l’hémorragie majeure à un an dans la fibrillation atriale. Le total ne constitue pas une contre-indication automatique à l’anticoagulation ; les définitions des facteurs et les recommandations contemporaines doivent correspondre à la version. Le calibrage et le traitement antithrombotique de la population influencent son interprétation.

## Références

- [Pisters R et al. A novel user-friendly score (HAS-BLED) to assess 1-year risk of major bleeding in patients with atrial fibrillation. Chest, 2010.](https://doi.org/10.1378/chest.10-0134)

- [Van Gelder IC et al. 2024 ESC Guidelines for the management of atrial fibrillation. Eur Heart J, 2024.](https://doi.org/10.1093/eurheartj/ehae176)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

Risque hémorragique élevé

| Détails du résultat | |
| --- | --- |
| Hémorragie majeure | 12,50 ou plus pour 100 patients-années |

Facteurs modifiables : contrôler la pression artérielle, stabiliser l’INR ou passer à un AOD, revoir les antiagrégants/AINS, réduire l’alcool.


### 2

Risque hémorragique élevé

| Détails du résultat | |
| --- | --- |
| Hémorragie majeure | 3,74 pour 100 patients-années |

Facteurs modifiables : contrôler la pression artérielle.


### 3

Risque hémorragique faible

| Détails du résultat | |
| --- | --- |
| Hémorragie majeure | 1,13 pour 100 patients-années |

