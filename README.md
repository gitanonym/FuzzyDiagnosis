# Fuzziness-Guided Diagnosis for Decision Tree Repair under Concept Drift

Decision trees are widely used in machine learning due to their interpretability, accuracy, and robustness.
However, when the underlying data distribution changes—a phenomenon known as concept drift—their performance can degrade significantly.

A common strategy to address this issue is to retrain the model on the newly drifted data. However, this approach does not provide insight into the nature of the change or how to repair the model more effectively.
In this work, we adopt a previously proposed methodology that first diagnoses the decision tree model to identify components most impacted by the concept drift, and then selectively repairs them.
Specifically, we propose a novel fuzziness-based diagnosis method that analyzes post-drift instances by considering both the features in each instance.

Evaluation on 57 benchmark datasets demonstrates that our method improves interpretability while maintaining competitive predictive performance compared to the previous method and traditional retraining methods.
These findings suggest that the proposed approach enables more robust concept drift handling and higher-quality model maintenance.

## This Repository is listed as:
- APPETITE - The algorithm, with baselines in it.
- Tester - All the files relevant to evaluate the algorithm, including configurations for each baseline diagnoser that ran.
- Data - The datasets with their descriptions.

## Reproduce:
To run the algorithm, all needed is:
1. Install the required packages as listed in the [environment yaml file]([URL](https://github.com/my-anonymous-git/spider_fuzzy_diagnosis/blob/main/environment.yml)). Third-party packages are: openpyxl, numpy, pandas, scipy, sklearn, sympy, shap.
2. Run test_all.py. test_all can get various parametrs to make the run parallel and more efficient. you can use the --help to check all out. The testing configuration for the baseline and the ablation test can be found in [TestingDiagnosersData.json](https://github.com/my-anonymous-git/spider_fuzzy_diagnosis/blob/main/Tester/TestingDiagnosersData.json).
3. That's it. The results will be saved in the results folder.


[Appendix of all the datasets can be located here](https://github.com/my-anonymous-git/spider_fuzzy_diagnosis/blob/main/data/all_datasets.csv)
    Good Luck!
