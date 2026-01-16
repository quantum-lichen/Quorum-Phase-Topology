# 🧬 Quorum-Phase-Topology : Transition de Phase Biologique

![Status: Research](https://img.shields.io/badge/Status-Research-blue.svg)
![Field: Biophysics](https://img.shields.io/badge/Field-Biophysics-green.svg)
![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-yellow.svg)

## 🎯 Synopsis
Ce dépôt documente la thèse du **Dr. Bryan Ouellette** stipulant que le **Quorum Sensing (QS)** n'est pas qu'un simple interrupteur génétique, mais une **transition de phase macroscopique** régie par la physique statistique hors-équilibre. En utilisant le formalisme de la matière active (Active Brownian Particles), nous démontrons l'isomorphisme entre les seuils de signalisation biochimique et les points critiques de percolation et de jamming.


## 📐 Formalisme Mathématique

### 1. Dynamique Individuelle (Équation de Langevin)
La dynamique d'une entité (bactérie ou robot) est définie par :
$$\dot{\mathbf{r}}_i = v(\bar{\rho}_i)\mathbf{n}_i + \sqrt{2D_T}\boldsymbol{\xi}_i$$
$$\dot{\theta}_i = \sqrt{2\nu_r}\zeta_i$$

Où $v(\bar{\rho}_i)$ représente la vitesse d'auto-propulsion dépendante de la densité locale, instaurant la boucle de rétroaction fondamentale du QS.

### 2. Condition de Transition MIPS
L'instabilité spinodale (Motility-Induced Phase Separation) se produit lorsque la vitesse chute de manière critique avec la densité :
$$\frac{d}{d\rho} [\rho v(\rho)] < 0$$

### 3. Diffusivité Effective
Le coefficient de diffusion macroscopique du système est :
$$D_{eff} = D_T + \frac{v^2}{2d\nu_r}$$

## 🔗 Architecture Causale du Système
```mermaid
graph TD
    A[Activité Métabolique] --> B[Auto-inducteur AI]
    B --> C[Concentration Locale V]
    C --> D[Expression Génétique]
    D --> E[Réduction Motilité v]
    E --> F[Accumulation/Jamming]
    F --> A
    F -- Seuil Critique --> G{Transition de Phase}
