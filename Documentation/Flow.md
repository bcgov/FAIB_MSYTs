![](D:/data/projects/MSYT/msyt_v4.0/Documentation/process_flow/process.png)

Figure 1. MSYT Process Flow

The MSYT process combines planted information derived from RESULTS with
the changes shown by the Forest Cover INV survey to account for ingress
and mortality. It is made up of a planted component and a natural
component.

## Planted Component

### Inputs

<table>
<thead>
<tr class="header">
<th style="text-align: left;">RESULTS Planting</th>
<th style="text-align: left;">SPAR</th>
<th style="text-align: left;">Provincial Site Productivity</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="text-align: left;">Opening Based</td>
<td style="text-align: left;">Genetic Worth</td>
<td style="text-align: left;">Site index by species</td>
</tr>
<tr class="even">
<td style="text-align: left;">Number Planted (by Species)</td>
<td style="text-align: left;"></td>
<td style="text-align: left;"></td>
</tr>
<tr class="odd">
<td style="text-align: left;">Area Planted (by Species)</td>
<td style="text-align: left;"></td>
<td style="text-align: left;"></td>
</tr>
</tbody>
</table>

### Outputs

<table>
<thead>
<tr class="header">
<th style="text-align: left;">Planted Component</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="text-align: left;">Opening based</td>
</tr>
<tr class="even">
<td style="text-align: left;">Planted Species Composition</td>
</tr>
<tr class="odd">
<td style="text-align: left;">Planted Density (initial)</td>
</tr>
<tr class="even">
<td style="text-align: left;">Planted Genetic Worth</td>
</tr>
<tr class="odd">
<td style="text-align: left;">Planting Delay</td>
</tr>
</tbody>
</table>

## Natural Component

### Inputs

<table>
<thead>
<tr class="header">
<th style="text-align: left;">RESULTS Forest Cover INV (Survey)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="text-align: left;">Opening based</td>
</tr>
<tr class="even">
<td style="text-align: left;">Natural Species Composition</td>
</tr>
<tr class="odd">
<td style="text-align: left;">Density (at survey, total sph)</td>
</tr>
</tbody>
</table>

### Outputs

<table>
<thead>
<tr class="header">
<th style="text-align: left;">Natural Component</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="text-align: left;">Opening based</td>
</tr>
<tr class="even">
<td style="text-align: left;">Species composition (as time of
survey)</td>
</tr>
<tr class="odd">
<td style="text-align: left;">Species density</td>
</tr>
</tbody>
</table>

## Assess for Ingress/Mortality

The planted composition is adjusted based on the Forest Cover INV survey
to account for ingress and mortality. The final species composition used
as input to a growth and yield model is comprised of both a planted and
a natural component.

<table>
<thead>
<tr class="header">
<th style="text-align: left;">Planted Component</th>
<th style="text-align: left;">Natural Component</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="text-align: left;">Planted Species Composition</td>
<td style="text-align: left;">Natural Species Composition</td>
</tr>
<tr class="even">
<td style="text-align: left;">Planted Density</td>
<td style="text-align: left;">Natural Density</td>
</tr>
<tr class="odd">
<td style="text-align: left;">Planted Genetic Worth</td>
<td style="text-align: left;"></td>
</tr>
<tr class="even">
<td style="text-align: left;">Planting Delay</td>
<td style="text-align: left;"></td>
</tr>
<tr class="odd">
<td style="text-align: left;">Percent Planted</td>
<td style="text-align: left;"></td>
</tr>
</tbody>
</table>

## GY Model inputs

The planted percent controls how much weight is assigned to the planted
component. There can be stands with either 100% planted or 0% planted. A
0% planted stand is treated as an natural stand and assigned random
spacing in the GY model.

## Yield Tables

-   derived from the GY model inputs
-   using TIPSY

------------------------------------------------------------------------

Author: D Waddell  
Date: Aug 30, 2022
