# Emotion Classification
A simple emotion classification using Multinomial Naive Bayes model

## Dataset Used
[CARER: Contextualized Affect Representations for Emotion Recognition](https://huggingface.co/datasets/dair-ai/emotion) (subset: unsplit):
- Paper url: [https://www.aclweb.org/anthology/D18-1404](https://www.aclweb.org/anthology/D18-1404)
- DOI: 10.18653/v1/D18-1404
- authors:
    - Saravia, Elvis  and
    - Liu, Hsien-Chi Toby  and
    - Huang, Yen-Hao  and
    - Wu, Junlin  and
    - Chen, Yi-Shin

## Model Performance
| Model | Accuracy | Macroaverage Recall Score | MacroAverage Precision Score | MacroAverage F1 Score |
|-------|-------|-----------|-------------|-------------|
| MNB | 87.2% | 76.8% | 87% | 80.1% |
| Decision Tree(max_depth=500) | 85% | 79.4% | 79.1% | 79.2% |
| Random Forest(max_depth=250, n_estimators=300) | 87.1% | 79.8% | 82.9% | 81.2% |
| CatBoost(depth=8, estimators=500, learning_rate=0.1) | 90.1% | 82.9% | 90.1% | 90.1% |