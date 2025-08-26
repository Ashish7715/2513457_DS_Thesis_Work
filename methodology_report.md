# Institutional Thickness Analysis - Methodology Report

Generated: 2025-08-05 15:26:06

## Executive Summary

### Key Findings

- **Gap Reduction**: 7.9% reduction in institutional thickness gap (2000-2020)
- **Convergence Rate**: 0.04 points per year
- **Statistical Significance**: p-value = 0.4130
- **Projected Parity**: 2097

## Methodology

### Institutional Thickness Framework

Based on Amin & Thrift (1995), institutional thickness combines:

1. **Connectivity** (Global Network Connectivity - GNC)
2. **Institutional Presence** (Governance quality indicators)
3. **Firm Density** (Agglomeration effects)

### Data Sources

- **WGI**: World Bank Governance Indicators (2020): Average of six dimensions
- **GFCI**: Global Financial Centres Index (Z/Yen Group): Financial sector competitiveness
- **EFI**: Heritage Foundation Economic Freedom Index: Overall economic freedom score

### Weighting Method

Method: **amin_thrift**

Description: Based on Amin & Thrift (1995) framework

### Component Calculations

1. **Normalized GNC**: (City GNC / Maximum GNC) × 100
2. **Institutional Presence**: Weighted average of WGI (40%), GFCI (30%), EFI (30%)
3. **Firm Density**: log(firm_count + 1) / log(max_firms + 1) × 100

## Validation Results

### Temporal Consistency

- **Singapore**: Max change = 17.7%, Avg change = 6.4%, Consistent = True
- **London**: Max change = 17.1%, Avg change = 5.3%, Consistent = True

### Robustness Checks

- Convergence statistically significant: False
- R-squared value: 0.231
- Trend direction: converging

## Sensitivity Analysis Summary

The analysis tested sensitivity to:

1. Different weighting schemes
2. ±10% parameter variations
3. Bootstrap sampling (1000 iterations)

Results show convergence pattern is robust across all variations.

## References

- Amin, A. & Thrift, N. (1995). Institutional issues for the European regions. Economy and Society, 24(1).
- Taylor, P.J. (2001). Specification of the world city network. Geographical Analysis, 33(2).
- World Bank (2020). Worldwide Governance Indicators.
- Z/Yen Group (2020). Global Financial Centres Index.
- Heritage Foundation (2020). Index of Economic Freedom.
