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

The statistical tests are provided in:
- Statistical tests
