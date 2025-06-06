# Land Use Land Cover Classification: Semi-Supervised Learning for Remote Sensing Images

A hybrid framework combining deep learning with interpretable decision trees for multi-label classification of remote sensing images with minimal labeled data.

## Key Contributions
- Developed **SSL-RForest** - an ensemble method achieving **84.69% AUPRC with just 1% labels** on DFC-15 dataset
- Integrated **EfficientNet feature extraction** with **Predictive Clustering Trees (PCTs)** for semi-supervised learning
- Designed novel variance function (`Var_f = w·Var(Y) + (1-w)·Var(X)`) to balance labeled/unlabeled data
- Demonstrated **20% improvement** over supervised baselines across 3 datasets (OPTIMAL-31, MLRSNet, DFC-15)
- Maintained model interpretability while matching deep learning performance

## Technical Highlights
- **Backbone CNNs**: ResNet-50 / EfficientNet-B2
- **SSL-PCT Algorithm**: Weighted variance minimization for tree construction
- **Ensemble Method**: 50-tree Random Forest
- **Metrics**: AUPRC, Accuracy (multi-label support)
