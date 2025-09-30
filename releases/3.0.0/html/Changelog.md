# MLDCAT-AP Changelog

## Introduction

This document describes the (major) changes to [the current version 2.1.0](https://semiceu.github.io/MLDCAT-AP/releases/2.1.0/) of the MLDCAT-AP for which a new version is being proposed ([version 3.0.0](https://semiceu.github.io/MLDCAT-AP/releases/3.0.0/)).

## Detailed changes from v2.1.0 to v3.0.0

The table below gives an overview of the classes (and their definitions) within both data models. Classes that are related are juxta-positioned.

**C** stands for changes in classes

**R** stands for changes in relationships

**P** stands for changes in properties

**D** stands for changes in data types

| Nr | MLDCAT-AP v2.1.0 | MLDCAT-AP v3.0.0 | Rationale | GitHub / Change |
| --- | --- | --- | --- | --- |
| - | - | Version 3.0.0 follow major version of DCAT-AP 3.X | - | - |
| C | it6:Risk | it6:HarmRisk | its own definition defines its more as an harm risk  | https://github.com/SEMICeu/MLDCAT-AP/issues/29 |
| C | - | it6:Modality | addition of this class to be compliant with the AI ACT and AI CoP | - |
| C | it6:Parameter | it6:Parameter | there were 2 classes Parameters, now simplified in one  | - |
| C | - | dct:Location | this class has been added to for the geographical coverage of the Dataset | - |
| C | it6:OutputFilePrediction | it6:File | this class has been renamed to include different files released   | - |
| R | - | dcat:DataService/it6:servesModel | addition of this relation to be compliant with the AI CoP | - |
| P | - | dcat:Dataset/it6:biasMethod | addition of this property to be compliant with the AI CoP  | - |
| P | - | dcat:Dataset/it6:curationMethod | addition of this property to be compliant with the AI CoP  | - |
| P | - | dcat:Dataset/it6:dataProvenance | addition of this property to be compliant with the AI CoP  | - |
| R | - | dcat:Dataset/dct:spatial | addition of this relation to be compliant with the AI CoP  | - |
| R | - | dcat:Dataset/dct:language | addition of this relation to be compliant with the AI CoP  | - |
| R | - | dcat:Dataset/dcat:theme | addition of this relation to be compliant with the AI CoP  | - |
| R | - | dcat:Dataset/dct:type| addition of this relation to be compliant with the AI CoP  | - |
| P | - | dcat:Dataset/it6:unsuitabilityMethod | addition of this property to be compliant with the AI CoP  | - |
| P |  dcat:Dataset/owl:versionInfo | dcat:Dataset/dcat:version | changes applied following DCAT-AP 3.0.1  | - |
| R |  dcat:Dataset/dct:MediaType | dcat:Dataset/dcat:mediaType | typo in the relation  | - |
| P | dcat:Distribution/dpv:hasData | dcat:Distribution/dpv:hasData | changing hyperling to the code list in the usage note  | https://github.com/SEMICeu/MLDCAT-AP/issues/25 |
| P | - | it6:EnvironmentalImpact/it6:measurementMethodology  | addition of this property to be compliant with the AI CoP  | - |
| P | it6:EstimationProcedure/it6:dataSplitsURL  | it6:EstimationProcedure/it6:hasSplit  | change property to relation to it6:Split  | https://github.com/SEMICeu/MLDCAT-AP/issues/16 |
| P | - | it6:Hardware/dct:description  | addition of this property to be compliant with the AI CoP  | - |
| P | - | it6:Library/dct:description  | addition of this property to be compliant with the AI CoP  | - |
| R | - | it6:Library/dct:isExecutedBy | to create a better relation with the File belonging to a Machine Learning Model  | - |
| P | - | it6:MachineLearningModel/it6:designSpecifications | addition of this property to be compliant with the AI CoP  | - |
| R | - | it6:MachineLearningModel/it6:hasInputModality | addition of this property to be compliant with the AI CoP and AI Act  | - |
| R | - | it6:MachineLearningModel/it6:hasOutputModality | addition of this property to be compliant with the AI CoP and AI Act  | - |
| R | it6:MachineLearningModel/it6:haRegisteredUser | it6:MachineLearningModel/it6:hasRegisteredUser  | typo in the relation | - |
| R | - | it6:MachineLearningModel/it6:methodOfDistribution | addition of this property to be compliant with the AI CoP and AI Act  | - |
| R | - | it6:MachineLearningModel/it6:modelArchitecture | addition of this property to be compliant with the AI CoP and AI Act  | - |
| P | - | it6:MachineLearningModel/it6:placedOnMarketDate | addition of this property to be compliant with the AI CoP  | - |
| P | - | it6:MachineLearningModel/it6:totalNumberOfParameters | addition of this property to be compliant with the AI CoP and AI Act | - |
| R | - | it6:Modality/it6:classification | addition of this property to be compliant with the AI CoP and AI Act | - |
| R | - | it6:Modality/it6:size | addition of this property to be compliant with the AI CoP | - |
| R | it6:Run/it6:hasEnvironmentalImpact | it6:Run/it6:hasInferencingImpact | specialized relation to be compliant with the AI CoP | - |
| R | it6:Run/it6:hasEnvironmentalImpact | it6:Run/it6:hasTrainingImpact | specialized relation to be compliant with the AI CoP and AI Act | - |
| R | it6:Run/it6:hasHyperParameter | it6:Run/it6:hasParameter | generalized relation to include different types of Parameter | - |
| P | -| it6:Run/it6:trainingTime | addition of this property to be compliant with the AI CoP | - |
| R | - | it6:Split/dct:type | added property to it6:Split  | https://github.com/SEMICeu/MLDCAT-AP/issues/16 |
| R | it6:MachineLearningModel/it6:hasMachineLearningLibrary | - | removal of this property to model differently | - |
| R | it6:MachineLearningModel/it6:hasTaskType | - | removal of this property to model differently | - |