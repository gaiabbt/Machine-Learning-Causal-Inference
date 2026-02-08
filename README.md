# Causal Inference with Machine Learning

University coursework (MSc Econometrics / Machine Learning).

Using a synthetic, school-clustered “mindset intervention” dataset, I estimated the average treatment effect (ATE) and compared machine-learning-based approaches for estimating the nuisance functions.

## What I did
- Implemented a cluster leave-one-school-out estimation procedure to reduce overfitting across schools
- Estimated nuisance components (outcome model and treatment propensity) using:
  - Random forests with simple feature selection
  - Gradient boosting (outcomes) and AdaBoost (propensity)
  - Small neural networks for both components, tuned with a basic search
- Computed orthogonal (doubly robust) ATE estimates per school and averaged across schools
- Performed basic diagnostics (overlap via propensity scores) and compared debiased versus non-debiased estimates

## Outputs
The notebook reports ATE estimates for each approach (random forest, boosting, neural networks) alongside a non-debiased baseline for comparison.
