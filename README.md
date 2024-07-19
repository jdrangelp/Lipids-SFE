# Machine Learning Regression Models to predict the lipid profile of supercritical extracts

Department of Biological Science, Universidad de los Andes, Bogotá, Colombia.

Product and Process Design Group, Department of Chemical and Food Engineering, Universidad de los Andes, Bogotá, Colombia.

# Introduction

This is a set of six machine learning regression models to predict the lipid profile of supercritical extracts from a microalgae (Galdieria sp. USBA-GBX-832) varying the conditions of temperature, pressure and cosolvent flow (ethanol). The regression models are Lasso, Support Vector Regressor, Gaussian Regression, Random Forest, XG Boost and ANN.

These models were built on may 2024 using the outcomes from the lipidomic characterization analysis of 12 supercritical extracts (through RP-LC-ESI(+/-)-QTOF-MS).

The input data is the defined extraction conditions: temperature (in °C), pressure (in bar) and ethanol flow (in mL/min), and the chemical structures in isomeric SMILES format. The output is the lipid recovery in Log[g lipid/ g biomass].

There is an optional input variable, the infinite dilution activity coefficient (IDAC) of the lipid calculated at the conditions of temperature and ethanol mole fraction. This variable was calculated using the thermodynamic software, JCOSMO, developed by LVPP from UFRGS, Brazil.

There is an intermediate step for obtaining the chemical structures of lipids without the highest identification level in the lipidomic analysis. It uses the reported structures with the same shorthand notation, then it is calculated the RD-Kit molecular descriptors and using an unsupervised learning method is selected the representative lipid. The structures fully described are used as the input by the models.

The methodology propused for building the models is restricted for predicting the lipid profile of the microalgae Galdieria sp. USBA-GBX-832, but researchers could follow this steps for predicting the lipid profiles of their biological samples used in SFE and reduce the cost and time needed to identify the optimal extraction conditions, whether to achieve the highest extraction yield or to optimize the recovery of specific lipids or lipid groups.

# Authors

Juan David Rangel Pinto¹*, Jose L. Guerrero², Lorena Rivera³, María Paula Parada-Pinilla³, Mónica P. Cala², Gina López³, Andrés Fernando González Barrios¹*

¹Grupo de Diseño de Productos Y Procesos (GDPP), Department of Chemical and Food Engineering, Universidad de los Andes, Bogotá, Colombia
²Metabolomics Core Facility—MetCore, Vice-Presidency for Research, Universidad de los Andes, Bogotá, Colombia
³Unidad de Saneamiento y Biotecnología Ambiental (USBA), Departamento de Biología, Facultad de Ciencias, Pontificia Universidad Javeriana (PUJ), Bogotá, Colombia

Corresponding Authors:
jd.rangel10@uniandes.edu.co; andgonza@uniandes.edu.co

#Cite us!

The paper will be submitted soon.
