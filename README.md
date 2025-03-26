# Depression

The features for one record are extracted in:

- Probabilities of euler angle single extraction
- Probabilities of eye and smiling single extraction
- AUs single extraction
- Facial features based on facial landmarks single extraction

The features for all records are extracted in:
- AUs extraction-all_loop
- Facial features based on facial landmarks-extraction-all_loop
- Probabilities of euler angle-extraction-all_loop
- Probabilities of eye and smiling extraction-all-loop

The cross-validation for one-leave-out-patient is provided in:
- Classification_AU
- Classification_euler
- Classification_prob_eye_features
- Classification_facial_features
- Classification_combination_all_features

The SHAP values for the best cross-validation for one-leave-out-patient is provided in:
- Classification_combination_all_features_SHAP

The preparation of features for nested cross-validation is provided in:
- for one record:
	* AUs single extraction-cross_single
	* Probabilities of euler angle-extraction-cross_single
	* Probabilities of eye and smiling-extraction-cross_single
 	* Facial features based on facial landmarks-extraction-cross_single

- for all records:
	* Probabilities of euler angle extraction-cross-all
	* Probabilities of eye and smiling extraction-cross_all
	* AUs single extraction-cross_all
 	* Facial features based on facial landmarks-extraction-cross_all

The nested cross-validation with Leave-One-Day-Out is provided in:
- AU classification - nested cross-valiadation 
- ff classification - nested cross-valiadation
- ff classification - nested cross-valiadation_updated (updated)
- AU classification - nested cross-valiadation_updated (updated)
- combination_features - nested cross-valiadation
- Euler classification - nested cross-valiadation
- Probabilities_eye_classification - nested cross-valiadation.ipynb

The SHAP values for the nested cross-validation with combined features for one-leave-day-out is provided in:
- SHAP_combination_features - nested cross-valiadation
- SHAP Euler classification - nested cross-valiadation

The ROC curves and Precision-Recall curves are generated for the multimodal approaches in:
- combination_features - nested cross-valiadation-ROC (for hybrid model)
- Classification_combination_all_features_ROC_universal (for universal model)


The results of the classification in the tables, SHAP values, likewise identified valuable features for each modality are gathered in the results folder:
- results_universal -> the outcomes for the universal model with Leave-One-Patient-Out for each modality and multimodality
- results_nested_cv -> the outcomes for the nested cross-validation with Leave-One-Day-Out for each modality and multimodality
- universal_model_features -> the most significant features identified with the usage of pyMRMR and pyHSICLasso libraries, for the scenario with the universal model, each modality and multimodality
- hybrid_model_feature -> the most significant features identified with the usage of pyMRMR and pyHSICLasso libraries, for the scenario with the hybrid model, each modality and multimodality
- ROC curves and Precision-Recall curves:
	- precision_recall_multi_nested_cv.pdf -> precision-recall curve for the multimdality and hybrid model
 	- ROC_multi_nested_cv.pdf -> ROC curve for the multimodality and hybrid model
 	- ROC_universal.pdf -> ROC curve for the multimodality and universal model
 	- precision_recall_multi_universal_cv.pdf -> precision-recall curve for the multimdality and universal model
- SHAP values:
	-  shap_combined_features_RF_patient_out_predict.pdf -> the SHAP values for the best universal model with Leave-One-Patient-Out, multimodal approach and Random Forest classifier
	-  shap_combined_features_RF_smote_patient_out_predict.pdf -> the SHAP values for the best universal model with Leave-One-Patient-Out, multimodal approach and Random Forest classifier and SMOTE
 	-  shap_combined_features_knn_smote_nest_predict.pdf -> the SHAP values for the best hybrid model with Leave-One-Day-Out, multimodal approach and k-NN classifier and SMOTE
  	-  shap_euler_knn_nest_predict.pdf -> the SHAP values for the second best hybrid model with Leave-One-Day-Out, Euler angles-related features, k-NN classifier
  	-  shap_euler_knn_smote_nest_predict.pdf -> the SHAP values for the best hybrid model with Leave-One-Day-Out, Euler angles-related features, k-NN classifier and SMOTE
  
  
The statistical tests are provided in:
- Statistical tests

The selection of valuable facial features was performed with:
-ff-all-features
