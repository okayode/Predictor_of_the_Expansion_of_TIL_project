# PETIL: Predicting Expansion of Tumor Infiltrating Lymphocytes for the Adoptive Cell Immunotherapy in Bladder Cancers

One major advance in treating solid tumors is the success of adoptive cell therapy (ACT), in which autologous tumor-infiltrating lymphocytes (TILs) are expanded and activated ex vivo and then reinfused into the cancer patient. 

PETIL is a tool that can first learn from patient and tumor data already collected in the clinic (local data) which data features are important for predicting TIL expansion, without the need to predefine which data categories to consider. Then, this tool predicts a possible TIL expansion for individual patients (personalized predictions), allowing to determine whether ACTTIL therapy could potentially treat an individual bladder cancer patient.


## PETIL needs the following libraries

```bash
numpy
sklearn
matplotlib
seaborn
pandas
tensorflow
statsmodels
scipy
```


## Repository structure
```text
.
├── 01_Data_summary.ipynb
├── 02_Data_table.ipynb
├── 03_norm.ipynb
├── 04a_midas_train.ipynb
├── 04b_midas_test.ipynb
├── 04c_Imputation_analysis.ipynb
├── 05_MI.ipynb
├── 06_p_corr.ipynb
├── 07a_FFS.ipynb
├── 07b_adeq_smplSz.ipynb
├── 07c_Stab_FeatSelection.ipynb
├── 08_MCC_RBF_SVM.ipynb
├── data
│   ├── baselinedata.csv
│   ├── BladderCancer_132P_TIL_prd1.xlsx
│   ├── norm_X_test_Yes_No_2.csv
│   ├── norm_X_test_Yes_No.csv
│   ├── norm_X_train_Yes_No_2.csv
│   ├── norm_X_train_Yes_No.csv
│   ├── Xy_test_Yes_No_md.csv
│   ├── Xy_Yes_No_md.csv
│   ├── y_test_Yes_No.csv
│   └── y_train_Yes_No.csv
├── Feature_Distri.ipynb
├── figs
│   ├── Age_at_Surgery.jpg
│   ├── aucroc_aucprroc_cv5.jpg
│   ├── BMI.jpg
│   ├── Fragments_plated.jpg
│   ├── his_01.jpg
│   ├── im_cv5_yes_no_2.jpg
│   ├── learning_curves_Yes_No2.jpg
│   ├── Sample_weight.jpg
│   ├── Stab_Analy_K_J.jpg
│   ├── Stab_Analy.jpg
│   ├── surf_cv5_yes_no_2.jpg
│   ├── Tumor_digest_count.jpg
│   ├── Yes_No_cm_2.jpg
│   ├── Yes_No_den_test.jpg
│   ├── Yes_No_den.jpg
│   ├── Yes_No_FFS.jpg
│   ├── Yes_No_ft.jpg
│   ├── Yes_No_MI.jpg
│   └── Yes_No_p_corr.jpg
├── midas
│   ├── __init__.py
│   ├── midas_base.py
│   └── my_midas.py
├── midas_ext
├── midas_test
│   ├── midas_test_0.csv
│   ├── midas_test_1.csv
│   ├── midas_test_10.csv
│   ├── midas_test_11.csv
│   ├── midas_test_12.csv
│   ├── midas_test_13.csv
│   ├── midas_test_14.csv
│   ├── midas_test_15.csv
│   ├── midas_test_16.csv
│   ├── midas_test_17.csv
│   ├── midas_test_18.csv
│   ├── midas_test_19.csv
│   ├── midas_test_2.csv
│   ├── midas_test_3.csv
│   ├── midas_test_4.csv
│   ├── midas_test_5.csv
│   ├── midas_test_6.csv
│   ├── midas_test_7.csv
│   ├── midas_test_8.csv
│   └── midas_test_9.csv
├── midas_train
│   ├── midas_train_0.csv
│   ├── midas_train_1.csv
│   ├── midas_train_10.csv
│   ├── midas_train_11.csv
│   ├── midas_train_12.csv
│   ├── midas_train_13.csv
│   ├── midas_train_14.csv
│   ├── midas_train_15.csv
│   ├── midas_train_16.csv
│   ├── midas_train_17.csv
│   ├── midas_train_18.csv
│   ├── midas_train_19.csv
│   ├── midas_train_2.csv
│   ├── midas_train_3.csv
│   ├── midas_train_4.csv
│   ├── midas_train_5.csv
│   ├── midas_train_6.csv
│   ├── midas_train_7.csv
│   ├── midas_train_8.csv
│   └── midas_train_9.csv
├── missing_test.csv
├── missing_train.csv
├── output_test.csv
├── output_train.csv
├── py_libraries.py
├── README.md
├── smpl_sz_adeq
│   ├── __init__.py
│   └── smpl_sz_adq.py
├── tmp
│   ├── checkpoint
│   ├── MIDAS
│   ├── MIDAS.data-00000-of-00001
│   ├── MIDAS.index
│   └── MIDAS.meta
└── utility
    ├── get_g_result.py
    ├── make_cm.py
    ├── mi_score.py
    ├── plt_result.py
    ├── sv_fig.py
    ├── sv_fig2.py
    └── sv_fig3.py
```

## Authors

Kayode Olumoyin kayode.olumoyin@moffitt.org, Katarzyna Rejniak 


## Source Code
https://github.com/okayode/Predictor_of_the_Expansion_of_TIL_project

## License


This project is licensed under the GNU General Public License v3.0.
