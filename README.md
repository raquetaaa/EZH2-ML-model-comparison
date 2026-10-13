# EZH2-ML-model-comparison
Recreational comparison of XGBoost and Random Forest regressors for prediction of pI50 values of small molecule drugs targeting enzyme EZH2 from the polycomb repressive complex 2 (PRC2)
**About the project**
* The EZH2 enzyme is in charge of silencing gene transcription by adding methyl groups to lysine 27 of histone H3. It is an interesting therapeutical target as it has been linked to histone methylation patterns leading to repression of tumor supressor genes in lymphoma, prostate cancer and breast cancer.
* pIC50 is the power of IC50, which measures the concentration needed to block a biological process by 50% _in vitro_. A higher pIC50 indicates a drug is more potent.
* Morgan fingerprints as bit vectors were used to train the model due to fit the models easily
* Mean average error (MAE) for Random Forest Regressor model was 0.427, while MAE for  XGBoost was 0.450, indicating good predictive accuracy for both.
* Used paired t-test via 5x2 fold cross validation to reduce type 1 errors by ensuring independence between samples. As p>0.05, there is no significant difference between prediction capacity of the regressors.
**Built with**
  *[CHEMBL_WEB_RESOURCE_CLIENT](https://github.com/chembl/chembl_webresource_client)
  * [RDKIT](https://www.rdkit.org/docs/)
  * [SKLEARN](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html)
  * [XGBOOST](https://xgboost.readthedocs.io/en/stable/)
  * [mlxtend](https://rasbt.github.io/mlxtend/)
