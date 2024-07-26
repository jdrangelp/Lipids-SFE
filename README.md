# Machine Learning Regression Models to predict the lipid profile of supercritical extracts

Department of Biological Science, Universidad de los Andes, Bogotá, Colombia.

Product and Process Design Group, Department of Chemical and Food Engineering, Universidad de los Andes, Bogotá, Colombia.

# Introduction

This study presents six machine learning regression models designed to predict the lipid profile of supercritical extracts from the microalgae Galdieria sp. USBA-GBX-832, varying conditions of temperature, pressure, and cosolvent flow (ethanol). The regression models used are Lasso, Support Vector Regressor, Gaussian Regression, Random Forest, XGBoost, and ANN.

These models were built in May 2024 using the outcomes from the lipidomic characterization analysis of 12 supercritical extracts obtained through RP-LC-ESI(+/-)-QTOF-MS.

The input data consist of defined extraction conditions: temperature (°C), pressure (bar), and ethanol flow (mL/min), along with the chemical structures in isomeric SMILES format. The output is the lipid recovery in Log[g lipid/g biomass].

An optional input variable is the infinite dilution activity coefficient (IDAC) of the lipid, calculated at the given temperature and ethanol mole fraction. This variable was computed using the thermodynamic software JCOSMO, developed by LVPP from UFRGS, Brazil.

An intermediate step is used to obtain the chemical structures of lipids that do not have the highest identification level in the lipidomic analysis. This step involves using reported structures with the same shorthand notation, calculating RDKit molecular descriptors, and selecting the representative lipid using an unsupervised learning method. The fully described structures are then used as input for the models.

The methodology proposed for building these models is specifically for predicting the lipid profile of Galdieria sp. USBA-GBX-832. However, researchers can follow these steps to predict the lipid profiles of their biological samples used in SFE, thereby reducing the cost and time needed to identify optimal extraction conditions, whether to achieve the highest extraction yield or to optimize the recovery of specific lipids or lipid groups.

# Authors

Juan David Rangel Pinto¹*, Jose L. Guerrero², Lorena Rivera³, María Paula Parada-Pinilla³, Mónica P. Cala², Gina López³, Andrés Fernando González Barrios¹*

¹Grupo de Diseño de Productos Y Procesos (GDPP), Department of Chemical and Food Engineering, Universidad de los Andes, Bogotá, Colombia
²Metabolomics Core Facility—MetCore, Vice-Presidency for Research, Universidad de los Andes, Bogotá, Colombia
³Unidad de Saneamiento y Biotecnología Ambiental (USBA), Departamento de Biología, Facultad de Ciencias, Pontificia Universidad Javeriana (PUJ), Bogotá, Colombia

Corresponding Authors:
jd.rangel10@uniandes.edu.co; andgonza@uniandes.edu.co

# Cite us!

The paper will be submitted soon.
