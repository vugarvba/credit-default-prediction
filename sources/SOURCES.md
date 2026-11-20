# Sources and provenance

## Dataset
UCI Machine Learning Repository: Default of Credit Card Clients (dataset 350)
https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients

Original study: Yeh, I-Cheng and Lien, Che-hui (2009), *The comparisons of data mining techniques for the predictive accuracy of probability of default of credit card clients*, Expert Systems with Applications.

## Metrics and figures
The validation metrics, test-set estimates, bootstrap intervals and confusion matrix were supplied from the author's executed Colab notebook in November 2026.
- Validation: logistic regression ROC-AUC .7190, PR-AUC .4946, Brier .1464; gradient boosting ROC-AUC .7808, PR-AUC .5484, Brier .1349.
- Holdout: ROC-AUC .7763 (CI .7623–.7916), PR-AUC .5512 (CI .5251–.5773), Brier .1355 (CI .1315–.1394).
- Confusion matrix: TN 2724, FP 1949, FN 298, TP 1029.
- Figure screenshots: `holdout_diagnostics.png`, `permutation_importance.png`, `partial_dependence.png`, `segment_calibration.png`, `segment_uncertainty.png`, `decision_cost_sensitivity.png` are from author's Colab visual outputs. `validation_model_comparison.png` was recreated from the validated displayed model comparison table.

These results have **not** been independently reproduced from an external dataset in this packaging environment.

## Methods
scikit-learn documentation: https://scikit-learn.org/stable/
Statsmodels Wilson CI: https://www.statsmodels.org/stable/generated/statsmodels.stats.proportion.proportion_confint.html
