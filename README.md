# ParameterOptimization_102217114

<h6> Dataset Selection </h6>
The Letter Recognition Dataset from the UCI Machine Learning Repository was selected. It contains 20,000 instances and 16 numerical attributes extracted from images of capital letters in the English alphabet (A–Z), making it a multi-class classification problem.

Preprocessing Steps
Label Encoding: The target column (letters) was encoded numerically using LabelEncoder.

Normalization: All feature values were scaled using StandardScaler to standardize their ranges.

Splitting: The dataset was divided into 10 different train-test splits with a 70:30 ratio, using stratified sampling to maintain class balance.

SVM Optimization
For each of the 10 samples, a population-based random search approach was used.

A total of 100 iterations were run per sample.

In each iteration:

SVM parameters (kernel, nu, epsilon) were randomly selected.

A NuSVC model was trained and tested.

Accuracy was recorded.

The best accuracy and corresponding parameters for each sample were stored.

For the sample with the highest accuracy, a convergence graph of accuracy vs. iteration was plotted.

<h2> Resultant table: </h2>

![image](https://github.com/user-attachments/assets/b6a5dfd7-eca9-4768-ac22-f791967e72f5)

<h2> Resultant graph: </h2>
![image](https://github.com/user-attachments/assets/55bf5bc1-aabb-4532-83a4-866ee765225d)

