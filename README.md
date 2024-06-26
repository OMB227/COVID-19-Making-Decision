# COVID-19-Making-Decision

![R badge](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)
![Git Badge](https://img.shields.io/badge/-Git-blue?style=flat&logo=Git&logoColor=white)

## Members

- Annette 
- Emmanuel A.
- Jay 
- Oumarou 
- Shama  
- Tiwonge
- Yvan 

## Title

The Impact of Timing of Non-Pharmaceutical Interventions (NPIs) on ICU Beds Occupancy During the 2020 COVID-19 Outbreak in Italy

## Objective

Our goal in this project is to advise Italian policymakers on the optimal timeline for interventions to prevent hospital
overcrowding, protect citizens by curbing the virus’s spread at the right time, and reduce public health costs for the government.

## Research Question
How does implementation of non-pharmaceutical interventions on days 5, 10, 30, and 50 after the first detected case of SARS-CoV-2 in Italy affect ICU bed occupancy?

## Description Data

The dataset containing historical data on COVID-19 cases, hospitalizations, and hospital bed occupancy has been sourced from the Italian National Institute of Health. Our dataset, named \texttt{hospitalization.csv}, includes 150 rows and 4 columns. Each row corresponds to a specific day starting from \emph{February 24, 2020} and includes the following columns:


<p align="center">
  <img src="images/excluded_icu.png" alt="non icu" width="300"/>
  <img src="images/icu.png" alt="icu" width="300"/>
</p>

## Model

<p align="center">
  <img src="images/Model diagram.jpg" alt="model" width="400"/>
</p>

## Differential Equation

\begin{align*}
\frac{dS}{dt} &= -\beta \frac{SI}{N} \\
\frac{dE}{dt} &= \beta \frac{SI}{N} - \sigma E \\
\frac{dI}{dt} &= \sigma E - \alpha I \\
\frac{dB_N}{dt} &= \alpha I - (\theta + \gamma_1) B_N \\
\frac{dB_{ICU}}{dt} &= \gamma_1 B_N - (\lambda_1 + \delta) B_{ICU}
\end{align*}



