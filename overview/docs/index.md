--- 
title: "MSYT Overview"
author: "Dave Waddell, MF, RPF"
date: "2023-03-01"
site: bookdown::bookdown_site
description: |
  This is the bookdown for the MSYT Overview
  The HTML output format for this example is bookdown::gitbook,
  set in the _output.yml file.
---


![](images/process.png)

Figure 1.  MSYT Process Flow


The MSYT process combines planted information derived from RESULTS with the changes shown by the Forest Cover INV survey to account for ingress and mortality.  It is made up of a planted component and a natural component.

## Planted Component

### Inputs

| RESULTS Planting | SPAR | Provincial Site Productivity |
|:-----------------|:------------|:-----------|
| Opening Based |  Genetic Worth | Site index by species | 
| Number Planted (by Species) | |
| Area Planted (by Species) | | NOT Spatially Located |



## Natural Component

### Inputs

| RESULTS Forest Cover INV (Survey) |
|:-------------------|
| Opening based |
| Natural Species Composition |
| Density (at survey, total sph) |
| Spatially separated into strata |


 
## Assess for Ingress/Mortality
  
The planted composition is adjusted based on the Forest Cover INV survey to account for ingress and mortality.  The final species composition used as input to a growth and yield model is comprised of both a planted and a natural component.

| Planted Component | Natural Component|
|:-------------------|:----------|
| Planted Species Composition | Natural Species Composition |
| Planted Density | Natural Density |
| Planted Genetic Worth | |
| Planting Delay | |
| Percent Planted | |


Note that the inclusion of both a planted component and a natural component differes significantly from base TIPSY.  


## GY Model inputs

The planted percent controls how much weight is assigned to the planted component.  There can be stands with either 100% planted or 0% planted.  A 0% planted stand is treated as an natural stand and assigned random spacing in the GY model.  

Mixed Plant : Natural Stands  
Mixed: Conifer : Deciduous  
Partially planted  


## Yield Tables

- derived from the GY model inputs
- using Batch TIPSY Composer

___

Author: D Waddell  
Date: Feb 21, 2023
