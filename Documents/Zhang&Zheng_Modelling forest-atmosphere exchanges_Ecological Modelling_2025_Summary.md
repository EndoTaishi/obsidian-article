# Zhang & Zheng (2025) - Modelling Forest-Atmosphere Exchanges Summary

**Title:** Modelling forest-atmosphere exchanges of carbon and water using an improved hydro-biogeochemical model in subtropical and temperate monsoon climates

**Authors:** Wei Zhang et al.

## Abstract/Introduction
Forest-atmosphere carbon exchanges are critical but challenging to quantify accurately. This study aimed to reduce uncertainties in forest carbon flux quantification by enhancing the CNMM-DNDC (Catchment Nutrient Management Model - DeNitrification-DeComposition) model. The enhancement involved developing a forest-specific growth module based on Biome-BGC formulations, with the goal of improving predictions of multiple ecosystem variables relevant to the United Nations Sustainable Development Goals (SDGs).

## Methodology

### Original Model (CNMM-DNDC)
The CNMM-DNDC model integrates soil carbon and nitrogen transformation processes into a distributed hydrological framework, simulating coupled carbon, nitrogen, and water cycles at catchment scales. It explicitly represents lateral water and nutrient transport.

### Improvements
The study enhanced the CNMM-DNDC model by incorporating a forest-specific growth module. This new module includes key processes such as photosynthesis, allocation, respiration, mortality, and litter decomposition, all based on Biome-BGC formulations. This addresses a limitation of the original model, which treated plants as an entirety, leading to uncertainties in forest carbon and nitrogen simulations.

### Validation
The improved model was evaluated against 8-year (2003-2010) eddy covariance data from three Asian forests (subtropical and temperate monsoon climates). The evaluation focused on simulations of daily Gross Primary Productivity (GPP), Ecosystem Respiration (ER), Net Ecosystem Exchange (NEE), and Evapotranspiration (ET).

### Sensitivity Analysis
Both one-at-a-time (OAT) and Morris global sensitivity analyses were conducted to assess the influence of new parameters and key input variables on the model's performance.

## Results/Findings

### Model Performance
- The updated model showed significant improvements over the original version.
- Normalized Root Mean Square Error (NRMSE) for GPP decreased by 46% and 54% at daily and annual scales, respectively. For ER, NRMSE decreased by 65% and 37%.
- Improvements in NEE were less pronounced due to error offsetting.
- The modified model better captured daily GPP dynamics and inter-annual variations, and significantly improved ER simulations across all sites.
- NEE simulations improved for CBM but remained comparable for QYZ and DHM.
- ET simulations showed significant improvements, especially at subtropical sites.
- Overall, the modified version reduced NRMSE by 38% and significantly increased Nash-Sutcliffe Efficiency (NSE) and R-squared (R2) across all evaluated flux variables.

### Sensitivity Analysis
- **Key Eco-physiological Parameters:** Specific leaf area (SLA, p30), fraction of leaf nitrogen in Rubisco (FLNR, p32), annual fraction of leaf and fine root turnover (LFRT, p6), and maximum stomatal conductance (gsmax, p33) were identified as most influential.
- **Meteorological Drivers:** Solar radiation was the predominant meteorological driver for GPP variations. Humidity and air temperature also had notable effects.
- **Soil Properties:** The model showed minimal sensitivity to soil properties.
- **Variability:** Parameter sensitivity varied depending on forest composition and climate regime (e.g., FLNR dominated in temperate mixed forests, while LFRT was more important in subtropical forests).

## Conclusions
The improved CNMM-DNDC model is a promising tool for quantifying multiple ecosystem variables relevant to SDGs, particularly with enhanced credibility in simulating forest carbon fluxes and budgets. While the model demonstrated robust performance in simulating GPP, ER, and ET, NEE simulations remain challenging. The study emphasizes the importance of component-specific validation to prevent error masking in net flux calculations and highlights the need for further verification and confirmation for comprehensive simulation of ecosystem variables for addressing multiple SDGs.