# offense_vs_pitching
**Offense vs. Pitching: An Analysis of Winning in Major League Baseball**
 
 This project analyzes whether offensive production or pitching performance is more strongly associated with team success in Major League Baseball. Using team-level data from 2015–2024, the analysis applies econometric methods to examine the relative relationships between standardized performance metrics and winning percentage.
The project emphasizes association rather than causation and demonstrates best practices in data cleaning, documentation, analysis, and visualization.


**Research Question**
 
 Which dimension of performance — offense or pitching — is more strongly associated with team winning percentage in Major League Baseball?


**Data Overview**

  •	Unit of analysis: Team–season
  
  •	Seasons included: 2015–2024 (2020 excluded)
  
  •	Sources:
  
> •	Performance metrics: FanGraphs, Sport Reference
>
> •	Payroll data: Spotrac
 
 Key variables include:
  
  •	Winning Percentage (WPct)
  
  •	Offensive performance (wRC+) (league average = 100, higher = better)
  
  •	Pitching performance (FIP−) (league average = 100, lower = better)
  
  •	Team payroll (log-transformed)
 
 A full data dictionary documenting variable definitions and transformations is included.


**Methodology**

  •	Ordinary Least Squares (OLS) regression framework
  
  •	Winning percentage modeled as a function of offensive and pitching performance
  
  •	Payroll included as a control for team resources
  
  •	Robustness checks using alternative performance metrics (OPS+, ERA−)
  
  •	All coefficients are interpreted as conditional associations, not causal effects.


**Limitations**

  •	Observational data does not support causal claims
  
  •	Team-level aggregation may mask within-team variation
  
  •	Defensive performance is not explicitly modeled
  
  •	Team and year fixed effects are not included and represent a potential extension

**Extensions**

 Future work could:
 
  •	Incorporate team and season fixed effects
  
  •	Use player-level data
  
  •	Explore event-based or within-team designs
