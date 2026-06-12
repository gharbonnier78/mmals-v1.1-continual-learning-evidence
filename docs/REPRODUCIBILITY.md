# Reproducibility

The repository stores compact derived evidence and key notebooks. Large raw score dumps and original 100+ MB run archives are excluded from normal GitHub hygiene.

## Primary runs

- SplitCIFAR10: RC2O-v2.2c robust, 5 seeds.
- SplitCIFAR100: RC2O-v2.2c robust diagnostic, 5 seeds.
- CORe50: RC2O-v2.2c robust diagnostic, 5 seeds.
- CORe50 v2.3: quick rescue ablation, seeds 0 and 4.

## Important protocol boundary

The external visual experiments train a supervised feature backbone on train-only data before the continual-learning sequence and then freeze it. Final-test data is reserved for evaluation. Candidate selection and repair use validation or repair memory only.
